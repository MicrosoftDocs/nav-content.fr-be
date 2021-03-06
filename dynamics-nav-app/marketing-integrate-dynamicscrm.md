---
title: "Gérer les clients à l'aide de Dynamics 365 for Sales"
description: "Vous pouvez utiliser Dynamics 365 for Sales depuis Dynamics NAV pour mapper les données et avoir une intégration et une synchronisation parfaites dans le processus allant du prospect à l'encaissement."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: integration, synchronize, map
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 3f26a80427a2a1c38949ca94848751527383d7f9
ms.contentlocale: fr-be
ms.lasthandoff: 10/26/2017

---
# <a name="managing-customers-and-sales-created-in-dynamics-365-for-sales"></a>Gestion des clients et des ventes créés dans Dynamics 365 for Sales
Si vous utilisez Dynamics 365 for Sales pour la communication avec le client, vous pouvez utiliser [!INCLUDE[d365fin](includes/d365fin_md.md)] pour le traitement des commandes et les finances et avoir une intégration transparente dans le processus allant du prospect à l'encaissement.

Lorsque votre application est configurée pour l'intégration à Dynamics 365 for Sales, vous avez accès aux données des ventes à partir de [!INCLUDE[d365fin](includes/d365fin_md.md)] et inversement dans certains cas. L'intégration vous permet d'utiliser et de synchroniser les types de données communs aux deux services, par exemple clients, contacts et informations de vente, et mettre à jour les données dans les deux emplacements.  

Par exemple, les commerciaux dans Dynamics 365 for Sales peuvent utiliser les tarifs dans [!INCLUDE[d365fin](includes/d365fin_md.md)] lorsqu'ils créent une commande vente. Lorsque ils ajoutent l'article à la ligne commande vente dans Dynamics 365 for Sales, ils peuvent également visualiser le niveau de stock (disponibilité) de l'article dans [!INCLUDE[d365fin](includes/d365fin_md.md)].

Inversement, les préparateurs de commandes dans [!INCLUDE[d365fin](includes/d365fin_md.md)] peuvent gérer les caractéristiques spéciales des commandes vente transférées automatiquement ou manuellement à Dynamics 365 for Sales, comme créer et valider automatiquement les lignes commande vente valides pour les articles ou les ressources qui ont été entrés dans les ventes en tant que produits hors catalogue. Pour plus d'informations, voir la section « Gestion des données de commandes vente spéciales ».  

> [!NOTE]
> Avant d'effectuer l'intégration à Dynamics 365 for Sales, vous devez effectuer diverses préparations techniques. Pour plus d'informations, consultez [Procédure : Configurer une connexion à Dynamics CRM](https://msdn.microsoft.com/en-us/dynamics-nav/how-to-set-up-a-dynamics-crm-connection) et [Procédure : Préparer Dynamics CRM pour l'intégration](https://msdn.microsoft.com/en-us/dynamics-nav/how-to-prepare-dynamics-crm-for-integration) sur MSDN.

## <a name="setting-up-the-connection"></a>Configuration de la connexion
À partir de la page d'accueil, vous pouvez accéder au guide de configuration assistée **Paramètres de connexion Dynamics 365 for Sales** qui vous aide à configurer la connexion. Une fois cette opération effectuée, vous disposez d'un couplage facile des enregistrements Dynamics 365 for Sales avec les enregistrements [!INCLUDE[d365fin](includes/d365fin_md.md)].  

> [!NOTE]  
> La section suivante explique la configuration assistée, mais vous pouvez effectuer les mêmes tâches manuellement dans la fenêtre **Paramètres de connexion Dynamics 365 for Sales**.

Dans le guide de configuration assistée, vous pouvez choisir les données à synchroniser entre les deux services. Vous pouvez également spécifier où vous souhaitez importer votre solution Dynamics 365 for Sales existante. Dans ce cas, vous devez indiquer les informations d'identification d'un compte utilisateur.

### <a name="setting-up-the-user-account-for-importing-the-solution"></a>Configuration du compte utilisateur pour importer la solution
Pour importer une solution Dynamics 365 for Sales existante, le guide d'installation utilise un compte administratif. Ce compte doit être un utilisateur valide dans Dynamics 365 for Sales avec les rôles de sécurité suivants :

* Administrateur système  
* Personnalisateur de solution  

Pour plus d'informations, voir [Créer des utilisateurs et attribuer des rôles de sécurité Microsoft Dynamics NAV (en ligne)](https://technet.microsoft.com/library/jj191623.aspx) sur techNet et [Procédure : gérer les utilisateurs et les autorisations](ui-how-users-permissions.md).  

Ce compte est uniquement utilisé lors de la configuration. Une fois la solution importée dans [!INCLUDE[d365fin](includes/d365fin_md.md)], le compte n'est plus nécessaire.

### <a name="setting-up-the-user-account-for-synchronization"></a>Configuration du compte utilisateur pour la synchronisation
L'intégration est basée sur un compte utilisateur partagé. Ainsi dans votre abonnement Office 365, vous devez créer un utilisateur dédié utilisé pour la synchronisation entre les deux services. Ce compte doit déjà être un utilisateur valide dans Dynamics 365 for Sales, mais vous n'avez pas à lui affecter de rôles de sécurité, car le guide de configuration le fait pour vous. Vous devez spécifier ce compte utilisateur à une ou plusieurs reprises dans le guide de configuration, en fonction du nombre de synchronisation que vous souhaitez activer. Pour plus d'informations, voir [Créer des utilisateurs et attribuer des rôles de sécurité Microsoft Dynamics NAV (en ligne)](https://technet.microsoft.com/library/jj191623.aspx) sur techNet.

Si vous décidez d'activer la *disponibilité de l'article*, le compte utilisateur intégration doit disposer d'une clé d’accès rapide des services Web. Cette opération s'effectue en deux étapes dans la page [!INCLUDE[d365fin](includes/d365fin_md.md)] de ce compte utilisateur, vous devez cliquer sur le bouton **Modifier la clé de service web** et dans le guide de configuration de la connexion Dynamics 365, vous devez spécifier cet utilisateur en tant qu'utilisateur de service Web OData.

Si vous décidez d'activer l'*intégration des commandes vente*, vous devez spécifier un utilisateur qui peut gérer cette synchronisation - un utilisateur de l'intégration ou un compte utilisateur différent.

### <a name="coupling-records"></a>Enregistrements couplage
Dans le guide de configuration assistée, vous pouvez choisir la synchronisation entre les deux services. Mais ultérieurement, vous pouvez également configurer la synchronisation de types spécifiques de données. Cette action est appelée le *couplage*, et cette section fournit des recommandations pour les éléments dont vous devez tenir compte.

Par exemple, si vous souhaitez afficher les comptes Dynamics 365 for Sales en tant que clients dans [!INCLUDE[d365fin](includes/d365fin_md.md)], vous devez coupler les deux types d'enregistrements. Ce n'est pas très compliqué, vous devez ouvrir la fenêtre **Liste des clients** dans [!INCLUDE[d365fin](includes/d365fin_md.md)] et il existe une action dans le ruban pour coupler ces données avec Dynamics 365 for Sales. Puis vous devez spécifier quels clients [!INCLUDE[d365fin](includes/d365fin_md.md)] correspondent à quels comptes dans Dynamics 365 for Sales.

Dans certains domaines, la fonctionnalité vous demande de coupler certains ensembles de données avant d'autres ensembles de données comme illustré dans la liste suivante :

* Clients et comptes  
  * Coupler d'abord des vendeurs avec des utilisateurs Dynamics 365 for Sales  
* Articles et ressources  
  * Coupler d'abord des unités de mesure avec des groupes d'unités Dynamics 365 for Sales  
* Prix des articles et des ressources  
  * Coupler d'abord des groupes tarifs client avec Dynamics 365 for Sales  

> [!NOTE]  
>   Si vous utilisez des tarifs en devises étrangères, assurez-vous de coupler des devises avec les devises de transaction Dynamics 365 for Sales.

Les commandes vente Dynamics 365 for Sales dépendent d'informations supplémentaires comme les clients, les unités de mesure, les devises, les groupes tarifs client, les articles et/ou les ressources. Pour que les commandes vente Dynamics 365 for Sales fonctionnent de façon transparente, vous devez d'abord coupler des clients, des unités de mesure, des devises, des groupes tarifs client, des articles et/ou des ressources.

### <a name="synchronizing-records-fully"></a>Synchronisation complète des enregistrements
À la fin du guide de configuration assistée, vous pouvez sélectionner l'action **Exécuter une synchronisation complète** pour démarrer la synchronisation de tous les enregistrements [!INCLUDE[d365fin](includes/d365fin_md.md)] avec tous les enregistrements associés de la solution Dynamics 365 for Sales connectée. Dans la fenêtre **Synchronisation complète CRM. Révision**, sélectionnez l'action **Démarrer**. La synchronisation commence à exécuter les projets en fonction des dépendances. Par exemple, les enregistrements de devise sont synchronisés avant les enregistrements client. La synchronisation complète peut durer longtemps et s'exécutera donc en arrière-plan afin que vous puissiez continuer à utiliser [!INCLUDE[d365fin](includes/d365fin_md.md)].

Pour vérifier la progression des projets individuels lors d'une synchronisation complète, accédez au champ **Statut écriture file d'attente des travaux**, **Statut projet Vers la table int.** ou **Statut projet À partir de la table int.** dans la fenêtre **Synchronisation complète CRM. Révision**.

Dans la fenêtre **Paramètres de connexion Dynamics 365**, vous pouvez obtenir des détails sur la synchronisation complète à tout moment. À partir de cette fenêtre, vous pouvez aussi ouvrir la fenêtre **Correspondances table intégration** pour afficher les détails des tables dans Dynamics NAV et dans la solution Dynamics 365 for Sales à synchroniser.

## <a name="handling-special-sales-order-data"></a>Gestion des données de commandes vente spéciales
Les commandes vente dans Dynamics 365 for Sales seront transférées à [!INCLUDE[d365fin](includes/d365fin_md.md)] automatiquement si vous sélectionnez la case à cocher **Créer automatiquement des commandes vente** dans la fenêtre **Paramètres de la connexion Microsoft Dynamics 365 for Sales**. Pour ces commandes vente, le champ **Nom** de la commande d'origine est transféré et associé au champ **Numéro de document externe** de la commande vente dans [!INCLUDE[d365fin](includes/d365fin_md.md)].

Ceci peut également fonctionner si la commande vente d'origine indique les biens hors catalogue, c'est-à-dire les articles ou les ressources qui ne sont enregistrés dans aucun produit. Dans ce cas, vous devez renseigner les champs **Type produit hors catalogue** et **N° produit hors catalogue** de la fenêtre **Paramètres ventes**, de sorte que ces ventes de produits non enregistrées soient mappées à un nombre donné d'articles/de ressources pour l'analyse financière.

Si la désignation de l'article sur la commande vente d'origine est très longue, alors une ligne commande vente supplémentaire de type Commentaire est créée pour stocker le texte intégral de la commande vente dans [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="see-also"></a>Voir aussi
[Gestion des relations](marketing-relationship-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Personnalisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)  
[Procédure : gérer les utilisateurs et les autorisations](ui-how-users-permissions.md)    
[Intégrer l'organisation et les utilisateurs dans Dynamics NAV (en ligne)](https://www.microsoft.com/en-US/Dynamics/crm-customer-center/onboard-your-organization-and-users-to-dynamics-365-online.aspx)  

##

