---
title: "Traitement des opportunités de vente"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 00f316dd3032d41239a75c0f40e6db6dc54601fe
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---
# <a name="processing-sales-opportunities"></a>Traitement des opportunités de vente
Une fois que vous avez créé une opportunité, il existe plusieurs fonctionnalités permettant de gérer l'opportunité et de la faire avancer jusqu'à l'achèvement.

## <a name="view-opportunities"></a>Afficher les opportunités
Les opportunités de vente existantes sont disponibles dans la fenêtre **Liste des opportunités**. Il existe différentes manières d'accéder à cette fenêtre pour le traitement des opportunités de vente :

|Pour afficher les opportunités pour |Alors |
|--------------------------|-----|
|Tous les vendeurs et contacts|Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Liste des opportunités**, puis sélectionnez le lien connexe.|
|Un vendeur spécifique|Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Vendeurs**, puis sélectionnez le lien connexe. Sélectionnez le vendeur, sélectionnez l'action **Opportunités**, puis l'action **Liste**.|
|Un contact spécifique|Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Contacts**, puis sélectionnez le lien connexe. Sélectionnez le contact dans la liste, puis sélectionnez l'action **Opportunités**.|

Chacune de ces tâches ouvre la fenêtre **Liste des opportunités**.

## <a name="close-opportunities"></a>Clôturer les opportunités
Vous pouvez clôturer des opportunités lorsque les négociations sont terminées. Lorsque vous clôturez une opportunité, vous pouvez spécifiez si elle a réussi ou échoué, et préciser les motifs de la clôture. Pour spécifier un motif, vous devez configurer des codes opportunité clôturée.

1. Dans la fenêtre **Liste des opportunités**, sélectionnez l'opportunité, puis sélectionner l'action **Clôturer**. La fenêtre **Terminer opportunité** s'affiche.
2. Renseignez les champs appropriés, puis cliquez sur le bouton **OK**.

  Les champs **Code fin opportunité** et **Date clôture** sont obligatoires. Vous devez les renseigner avant de cliquer sur le bouton **OK**.

  Dans le champ **Code fin opportunité**, vous pouvez choisir l'un des codes fin opportunité existants ou en ajouter un nouveau. Pour ajouter un nouveau code, dans la liste déroulante, sélectionnez **Sélectionner dans la liste complète**, puis sélectionnez **Nouveau**. Dans la nouvelle ligne vierge, renseignez les champs **Code**, **Type** et **Désignation**, puis cliquez le bouton **OK**.

## <a name="create-quotes-for-opportunities"></a>Créer des devis pour les opportunités
Vous pouvez créer des devis pour les contacts qui ne sont pas enregistrés en tant que clients.

1. Dans la fenêtre **Liste des opportunités**, sélectionnez l'opportunité, puis sélectionner l'action **Créer devis**. La fenêtre **Devis** s'affiche.
2. Renseignez les champs de votre choix.

## <a name="create-sales-orders-for-opportunities"></a>Créer des commandes vente pour les opportunités
Vous pouvez effectuer des commandes vente à partir des devis que vous avez créés pour vos opportunités. Pour pouvoir créer des commandes vente pour vos contacts, vous devez créer le contact en tant que client. Pour plus d'informations, reportez-vous à [Créer un client, un fournisseur ou un compte bancaire à partir d'un contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).

1. Dans la fenêtre **Liste des opportunités**, recherchez l'opportunité pour laquelle vous avez créée un devis vente.
2. Sélectionnez les actions Créer devis. La fenêtre **Devis** s'ouvre et affiche le devis que vous avez affecté à l'opportunité.
3. Renseignez les autres champs, puis sélectionnez l'action **Créer commande**.

Lorsque vous traitez des opportunités de vente, vous pouvez être amené à créer un devis pour le contact auquel est liée l'opportunité.

## <a name="delete-opportunities"></a>Supprimer des opportunités
Vous pouvez supprimer des opportunités, par exemple après avoir conclu un marché. Toutefois, vous pouvez uniquement supprimer des opportunités clôturées. Il existe deux méthodes permettant de supprimer des opportunités clôturées. Vous pouvez supprimer des opportunités clôturées une par une à partir de la fenêtre **Liste des opportunités**, ou vous pouvez exécuter le traitement par lots **Supprimer les opportunités clôturées** afin de supprimer plusieurs opportunités sur la base de critères spécifiés.

Pour supprimer des opportunités clôturées à partir de la fenêtre **Liste des opportunités**, sélectionnez l'opportunité, puis sélectionnez l'action **Supprimer**.

Pour supprimer des opportunités clôturées à l'aide du traitement par lots **Supprimer les opportunités clôturées**, procédez comme suit :

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Supprimer opportunités**, puis sélectionnez le lien connexe.
2. Dans la section **Opportunité**, configurez les filtres qui spécifient les opportunités clôturées à supprimer.
3. Cliquez sur le bouton **OK**.

Une fois que vous avez supprimé une opportunité, elle ne s'affiche plus dans la fenêtre **Liste des opportunités**.

## <a name="move-an-opportunity-through-sales-cycle-stages"></a>Faire avancer une opportunité au fil des étapes du cycle de vente
Si une opportunité suit un cycle de vente, vous pouvez la faire avancer ou reculer au fil des différentes étapes, par exemple la faire passer à l'étape suivante ou précédente, et même ignorer une étape.

1. Dans la fenêtre **Liste des opportunités**, sélectionnez l'action **Mettre à jour**. La fenêtre **Mise à jour opportunité** s'affiche.
2. Utilisez le champ **Type action** pour faire avancer l'opportunité au fil des étapes du cycle de vente :
  * **Suivant** fait avancer l'opportunité d'une étape.
  * **Ignorer** fait avancer l'opportunité d'une ou de plusieurs étapes dans le cycle de vente, que vous spécifiez dans le champ **Présentation**. Vous pouvez uniquement ignorer les étapes qui ont été configurées de sorte à l'autoriser.
  * **Précédent** fait reculer l'opportunité d'une étape.
  * **Omettre** fait reculer l'opportunité d'une ou de plusieurs étapes dans le cycle de vente, que vous spécifiez dans le champ **Présentation**.
  * **Mettre à jour** vous permet de modifier les informations (par exemple pour modifier votre évaluation de leurs chances de succès et valeurs estimées) sans passer à une autre étape.
3. Renseignez autres champs selon vos besoins, puis cliquez sur le bouton **OK**.

##<a name="see-also"></a>Voir aussi  
[Gestion des ventes](sales-manage-sales.md)  
[Création et gestion de contacts](marketing-contacts.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

