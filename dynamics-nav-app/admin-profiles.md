---
title: Gestion des profils et tableaux de bord
description: "Découvrez comment gérer les utilisateurs et les tableaux de bord dans Dynamics NAV."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, roles, role centers, user roles
ms.date: 09/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cd60cbc206b8e2cd6665b98ee49a5dc10c50fe08
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="managing-profiles-and-role-centers"></a>Gestion des profils et tableaux de bord
Les profils sont des collections d'utilisateurs [!INCLUDE[navnow_md](includes/navnow_md.md)] qui partagent le même tableau de bord. Un tableau de bord est un type de page dans lequel vous pouvez placer différentes sections. Chaque section est un conteneur dans lequel vous pouvez héberger d'autres pages ou sections prédéfinies du système, telles qu'une ou des sections d'Outlook afin d'ajouter des tâches, des notifications ou des notes.  

## <a name="about-profiles-and-role-centers"></a>À propos des profils et des tableaux de bord
Les profils permettent de lier les utilisateurs aux Tableaux de bord prédéfinis. Un Tableau de bord est une page d'accueil pour tous les utilisateurs d'un profil, qui a été configurée pour mettre en avant les tâches et les priorités des utilisateurs du profil. Par exemple, le Tableau de bord de préparateur de commandes a été configuré pour tenir compte des tâches et les priorités d'un préparateur de commandes. Un Tableau de bord fournit un accès facilité aux informations dont les utilisateurs ont besoin pour effectuer leur travail quotidien. Par exemple, le Tableau de bord détermine les piles, ou mosaïques, qui s'affichent lorsque les utilisateurs se connectent pour la première fois, ainsi que les liens à partir de la page de navigation.

Le profil utilisé s’affiche dans l’en-tête de la zone de contenu du tableau de bord. Un administrateur peut personnaliser le Tableau de bord pour qu'il corresponde à un rôle spécifique d'une société spécifique. Le Tableau de bord de préparateur de commandes peut ensuite être encore personnalisé sur un seul ordinateur pour satisfaire les besoins d'une personne qui va effectuer le travail de préparateur de commandes. Cette personne peut personnaliser le Tableau de bord pour enregistrer des requêtes, ajouter des filtres, et ajouter ou supprimer des champs.

Les profils et les Tableaux de bord s'alignent avec les rôles et responsabilités de votre organisation. [!INCLUDE[navnow_md](includes/navnow_md.md)] offre un ensemble de profils par défaut, chacun étant lié à un Tableau de bord. Les administrateur peuvent modifier les profils existants ou en créer de nouveaux.  
  
> [!NOTE]  
>  bien que les profils utilisateur ne soient pas explicitement liés aux rôles et autorisations constituant le système de sécurité, ils doivent disposer d'autorisations alignant leurs rôles à ce système. Pour plus d'informations, voir [Sécurité de l'environnement personnalisé](http://go.microsoft.com/fwlink?LinkId=147633) dans MSDN Library. 

## <a name="to-create-a-profile"></a>Pour créer un profil
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Profils**, puis sélectionnez le lien connexe.  
  
2.  Sélectionnez l'action **Nouveau** pour ouvrir la fenêtre **Fiche nouveau profil**.  
  
3.  Dans le champ **ID profil**, entrez un nom qui décrit le rôle prévu pour l'utilisateur.  
  
4.  Dans le champ **Description**, entrez une description de l'ID profil, par exemple, **Préparateur de la commande**.  
  
5.  Définissez le champ **ID Tableau de bord** sur le Tableau de bord à affecter au profil.  
  
6.  Pour configurer le Tableau de bord comme profil par défaut, activez la case à cocher **Tableau de bord par défaut**.  
  
7.  Cliquez sur le bouton **OK**. .  
  
La procédure à suivre pour modifier un profil existant est la même, à la différence près que vous sélectionnez un profil existant dans la page Profils au lieu de cliquer sur **Nouveau**.  


##<a name="copying-a-profile"></a>Copier un profil 
La copie d'un profil vous permet de gagner du temps si vous voulez utiliser des paramètres similaires pour un profil et modifier uniquement certains paramètres.

1.  Ouvrez le profil que vous voulez copier, puis sélectionnez l'action **Copier le profil**.

2.  Dans le champ **ID nouveau profil**, entrez un nom pour le profil que vous voulez copier. 

3.  Définissez le champ **Portée du nouveau profil** comme l'un des éléments suivants :

    - **Système** pour rendre le nouveau profil disponible à toutes les bases de données d'abonné qui utilisent l'application.
    - **Abonné** pour rendre le nouveau profil disponible uniquement à la base de données actuelle de l'abonné. 
4. Lorsque vous avez terminé, sélectionnez le bouton **OK**.

## <a name="ExportImportProfile"></a>Exportation et importation de profils

Vous pouvez exporter et importer des profils en tant que fichiers XML depuis et vers une base de données [!INCLUDE[d365fin](includes/d365fin_md.md)]. L'exportation et l'importation de profils vous permettent de gagner du temps lors de la configuration de l'interface utilisateur, car vous réutilisez une configuration de profil existante au lieu d'en configurer un en partant de zéro. Si vous avez un profil qui est configuré dans une base de données [!INCLUDE[d365fin](includes/d365fin_md.md)] et que vous souhaitez réutiliser tout ou partie de cette configuration dans une autre base de données, vous pouvez exporter le profil vers un fichier XML. Ensuite, vous pouvez importer le fichier XML du profil dans l'autre base de données.

-   Pour exporter un profil, ouvrez la recherche et ouvrez la page **Exporter les profils**, sélectionnez le profil dans la liste, puis sélectionnez l'action **Exporter**. Enregistrez le fichier XML dans un emplacement de votre ordinateur ou du réseau. 
  
-   Pour importer un profil, ouvrez la recherche et ouvrez la page **Importer les profils**, sélectionnez le fichier XML, puis sélectionnez le bouton **OK**. 

    > [!NOTE]  
    >  Vous ne pouvez pas importer un profil existant déjà dans la base de données, même si le fichier XML est nommé ou contient un contenu différent. Vous devez supprimer le profil existant avant de pouvoir importer le nouveau profil. 



## <a name="see-also"></a>Voir aussi  
[Procédure : gérer les utilisateurs et les autorisations](ui-how-users-permissions.md)  
[Personnalisation de l’interface utilisateur](ui-customizing-overview.md)   
<!--[Security Overview](../Security%20Overview.md)-->

