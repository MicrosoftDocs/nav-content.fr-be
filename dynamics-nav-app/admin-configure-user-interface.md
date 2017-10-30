---
title: Configuration de l'interface utilisateur (IU) pour les utilisateurs
description: "En tant qu'administrateur, configurez les interfaces utilisateur par défaut de la société en personnalisant les présentations des différents profils utilisateur de la société."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize pages, configure user interface, customize UI
ms.date: 07/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ba3d45a856eb38fe99fc5012b4e2f2d8609f9ce
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="configuring-the-user-interface-ui-for-users"></a>Configuration de l'interface utilisateur (IU) pour les utilisateurs
En tant qu'administrateur, vous configurez les interfaces utilisateur par défaut de la société en personnalisant les présentations des différents profils utilisateur de la société. Pour exécuter ce travail, vous devez être un administrateur avec la permission SUPER définie. De plus, les profils doivent être paramétrés et les utilisateurs correspondants leur être affectés. Pour plus d'informations, voir [Gestion des utilisateurs, des profils et des tableaux de bord](admin-users-profiles-roles.md).  
  
Vous configurez l'interface utilisateur pour plusieurs utilisateurs en personnalisant les pages pour un profil particulier auquel les utilisateurs sont affectés. Procédez à l'aide de [!INCLUDE[nav_windows](includes/nav_windows_md.md)], et effectuez la personnalisation de la même manière que les utilisateurs particuliers personnalisent leurs propres espaces de travail, c'est-à-dire à l'aide de la fonctionnalité **Personnaliser**. La différence est que vous ouvrez [!INCLUDE[nav_windows](includes/nav_windows_md.md)] en mode configuration. Les personnalisations courantes comprennent les actions à inclure dans le ruban, la manière dont les champs sont placés dans Raccourcis ou dans Récapitulatifs, et les éléments de menu à inclure dans le volet de navigation. 

> [!TIP]  
>  Une méthode rapide pour implémenter des configurations d'IU pour un profil est possible si vous avez déjà un profil configuré dans une autre base de données [!INCLUDE[d365fin](includes/d365fin_md.md)]. Vous pouvez alors exporter ce profil, puis l'importer dans la base de données actuelle. Pour plus d'informations, voir [Exportation et importation de profils](admin-profiles.md#ExportImportProfile).  
  
## <a name="general-information"></a>Informations générales
Tenez compte des informations suivantes avant de commencer à configurer l'interface utilisateur :
-   avant de configurer l'IU, l'application peut être configurée de sorte à afficher et masquer des éléments de l'interface utilisateur (par exemple des champs, des organisateurs et des récapitulatifs) en fonction de la licence ou des autorisations de l'utilisateur. Pour plus d'informations sur cette procédure, voir [Suppression de composants de l'interface utilisateur conformément aux autorisations](https://msdn.microsoft.com/en-us/dynamics-nav/removing-elements-from-the-user-interface-according-to-permissions).

    Pour voir l'effet de l'option Suppression d'éléments de l'interface utilisateur, vous pouvez vous connecter en tant qu'utilisateur de test avec l'autorisation définie du profil que vous configurez. La raison est que vous, en tant qu'administrateur, bénéficiez de l'ensemble d'autorisations SUPER, et vous ne pouvez donc pas afficher ni tester l'interface utilisateur résultante au cours de votre propre connexion.    
-   Lorsque vous apportez des modifications à la configuration de l'interface utilisateur pour une page qu'un utilisateur a personnalisée, la personnalisation de l'interface utilisateur de l'utilisateur est conservée, et n'est pas remplacée par la nouvelle configuration de page. De même, lorsque vous annulez votre configuration de l'interface utilisateur d'une page qu'un utilisateur a personnalisé depuis, la personnalisation de l'interface utilisateur de l'utilisateur n'est pas annulée.
-   La seule situation où la configuration de l'interface utilisateur remplace la personnalisation de l'interface utilisateur est lorsqu'un élément de l'interface utilisateur est supprimé par la configuration. Par exemple, si l'administrateur supprime un champ que l'utilisateur a renommé ou déplacé, le champ est toujours supprimé de l'interface utilisateur de l'utilisateur.
-   Vous pouvez enregistrer des configurations de l'interface utilisateur de la même page en fonction des différents points d'accès à la page. Par exemple, la fenêtre **Commandes vente** peut être personnalisée de manière à être différente lorsqu'elle est ouverte depuis la fenêtre **Fiche client** que lorsqu'elle est ouverte à partir du Tableau de bord **Préparateur de commandes vente**. Le point à partir duquel vous accédez à la page à personnaliser est enregistré dans cette personnalisation de page spécifique. Par conséquent, il peut y avoir plusieurs enregistrements de personnalisation de page dans la base de données, comme vous pouvez le voir dans la fenêtre **Supprimer la configuration du profil**.  
-   Contrairement à la possibilité des utilisateurs de modifier la taille des fenêtres ou la largeur des colonnes sur leur propre ordinateur, de telles modifications de vue basiques que vous apportez au cours de votre configuration de l'interface utilisateur pour un profil ne sont pas enregistrées sur le profil et ne sont pas disponibles pour les utilisateurs affectés au profil. Les modifications d'affichage de base sont spécifiques à l'ordinateur.   

## <a name="configure-a-profile-with-the-includenavwindowsincludesnavwindowsmdmd-in-configuration-mode"></a>Configurer un profil avec [!INCLUDE[nav_windows](includes/nav_windows_md.md)] en mode configuration
1.  Ouvrez une invite de commandes, puis saisissez la commande suivante pour changer le dossier d'installation de [!INCLUDE[nav_windows](includes/nav_windows_md.md)]. Par exemple :  
  
    ```  
    cd C:\Program Files\(x86)\Microsoft Dynamics NAV\110\RoleTailored Client  
    ```  
  
2.  Entrez la commande suivante pour démarrer [!INCLUDE[nav_windows](includes/nav_windows_md.md)] en mode configuration pour un profil spécifique :  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"profileid"  
    ```  
  
     Remplacez **profileid** par le nom du profil que vous voulez configurer.  
  
     Par exemple, pour configurer le profil de Responsable de la comptabilité, utilisez la commande suivante :  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"Accounting Manager"  
    ``` 

3. Vous pouvez maintenant commencer à configurer l'interface utilisateur, ce que vous faites de la même manière que les utilisateurs particuliers personnalisent leurs propres espaces de travail. Pour plus d'informations, voir [Personnalisation de votre espace de travail dans [!INCLUDE[nav_windows](includes/nav_windows_md.md)]](ui-personalization-windows-client.md). 

## <a name="cancel-ui-configuration"></a>Annuler la configuration de l'interface utilisateur
Vous pouvez annuler des personnalisations de l'interface utilisateur que vous avez créées comme configuration d'un profil de trois manières :  
  
-   Annulez toutes les personnalisations de l'interface utilisateur que vous avez créées pour un profil à l'aide du bouton **Effacer les pages configurées** dans la fenêtre **Fiche profil**.  
  
-   Annulez la personnalisation de l'interface utilisateur que vous avez créée pour les pages spécifiques d'un profil en supprimant des lignes de la fenêtre **Supprimer la configuration du profil**.  
  
-   Annulez la personnalisation de l'interface utilisateur que vous avez créée pour une zone d'interface utilisateur spécifique dans une page spécifique d'un profil à l'aide du bouton **Rétablir les valeurs par défaut** dans la fenêtre **Personnaliser**.  
  
### <a name="general-information"></a>Informations générales  
-   Les utilisateurs peuvent effectuer des personnalisations de l'interface utilisateur sous leur propre identifiant utilisateur pour personnaliser leur interface utilisateur. Lorsque vous annulez votre configuration de l'interface utilisateur d'une page qu'un utilisateur a personnalisé depuis, la personnalisation de l'interface utilisateur de l'utilisateur n'est pas annulée. De même, lorsque vous créez une nouvelle configuration de l'interface utilisateur pour une page qu'un utilisateur a personnalisée, une personnalisation de l'interface utilisateur de l'utilisateur est conservée, et n'est pas remplacée par la nouvelle configuration de page.  

    La seule situation où la configuration de l'interface utilisateur remplace la personnalisation de l'interface utilisateur est lorsqu'un élément de l'interface utilisateur est supprimé par la configuration. Par exemple, si l'administrateur supprime un champ que l'utilisateur a renommé ou déplacé, le champ est toujours supprimé de l'interface utilisateur de l'utilisateur.  
  
-   Dans la fenêtre **Supprimer la personnalisation utilisateur** et à l'aide du bouton **Rétablir les valeurs par défaut** dans la fenêtre **Personnaliser**, les utilisateurs peuvent annuler une personnalisation de l'interface utilisateur qu'ils ont créée sur des pages dans leur propre connexion utilisateur. Lorsque c'est le cas, la présentation de ces pages est réinitialisée sur n'importe quelle personnalisation de l'interface utilisateur que l'administrateur a configurée pour le profil. Si le profil n'a pas été configuré, la présentation des pages de l'utilisateur est réinitialisée à la configuration du profil par défaut. Pour plus d'informations sur la manière dont les utilisateurs annulent leur personnalisation, voir [Annuler la personnalisation](ui-personalization-windows-client.md#CancelPersonalization).
  
### <a name="to-cancel-all-ui-customization-that-you-have-made-for-a-profile"></a>Pour annuler toutes les personnalisations de l'interface utilisateur que vous avez créées pour un profil  
  
1.  Dans la zone **Rechercher**, saisissez **Profils**, puis sélectionnez le lien associé.  
  
2.  Sélectionnez le profil pour lequel vous souhaitez annuler toutes les personnalisations de l'interface utilisateur, puis, sous l'onglet **Accueil**, dans le groupe **Gérer**, sélectionnez **Modifier**.  
  
3.  Dans la fenêtre **Fiche profil**, sous l'onglet **Actions**, dans le groupe **Fonctions**, choisissez **Effacer les pages configurées**.  
  
> [!NOTE]  
>  Toutes les personnalisations de l'interface utilisateur pour le profil, aussi bien celles qui ont été installées avec l'application que celles créées par l'administrateur, sont annulées. Aucune mise en page spécifique au profil ne reste dans la base de données.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-specific-page-for-a-profile"></a>Pour annuler la personnalisations de l'interface utilisateur que vous avez créée une page spécifique d'profil  
  
1.  Dans la zone **Rechercher**, entrez **Supprimer la configuration du profil**, puis choisissez le lien associé.  
  
2.  Sélectionnez le profil/la page pour lequel/laquelle vous souhaitez annuler la personnalisation de l'interface utilisateur, puis, sous l'onglet **Accueil**, dans le groupe **Gérer**, sélectionnez **Supprimer**.  
  
    > [!IMPORTANT]  
    >  Si vous avez configuré des personnalisations de l'interface utilisateur de la même page en fonction des différents chemins d'accès de navigation à cette page, la personnalisation de chaque page est répertoriée dans la fenêtre **Supprimer la configuration du profil** avec les mêmes informations. Il n'existe aucune information pour identifier quelle ligne est liée à quel chemin d'accès de navigation. Par conséquent, vous devez supprimer les lignes une à une suivies de vérifications visuelles sur la page, ou vous pouvez supprimer toutes les lignes présentant des personnalisations de l'interface utilisateur pour le profil/page.
    >    
    >  Toutes les personnalisations de l'interface utilisateur pour la page de profil que vous avez effectuées lors de l'installation, ou depuis la dernière fois que vous avez utilisé la fenêtre **Supprimer la configuration du profil**, sont annulées. La disposition de la page est réinitialisée à la présentation standard de l'objet de page.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-a-specific-ui-area-for-a-specific-page-for-a-profile"></a>Pour annuler une personnalisation de l'interface utilisateur que vous avez créée pour une région spécifique de l'interface utilisateur pour une page spécifique d'un profil  
  
Vous pouvez annuler les modifications que vous avez apportées aux zones de l'interface utilisateur individuelles, comme un ruban, à l'aide du bouton **Restore Defaults** de la fenêtre **Customize**. Sinon, vous pouvez annuler toutes les modifications d'interface utilisateur que vous avez apportées à un profil via la fenêtre **Supprimer la configuration du profil**.  
  
La personnalisation de l'interface utilisateur pour le profil de la région particulière de l'interface utilisateur sur la page donnée est annulée. La disposition de la zone d'interface utilisateur sur la page est réinitialisée à la configuration par défaut pour votre profil, telle que réalisée par l'administrateur ou installée avec l'application.  
  
## <a name="see-also"></a>Voir aussi  
[Personnalisation de [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-customizing-overview.md)   
