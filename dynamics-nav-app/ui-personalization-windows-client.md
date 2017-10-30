---
title: Personnalisation de pages dans le client Windows Dynamics
description: "Découvrez comment personnaliser l'interface utilisateur pour l'adapter à votre méthode de travail."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 12aee74950066647f61639ec88c47e9be3c2f172
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace-in-the-dynamics-windows-client"></a>Personnalisation de votre espace de travail dans le client Windows Dynamics
Vous pouvez personnaliser votre espace de travail pour l'adapter à vos habitudes et préférences en modifiant les pages afin qu'elles n'affichent que les informations dont vous avez besoin, où vous avez en besoin. Les modifications de personnalisation que vous apportez n'affectent que ce que vous voyez, pas ce que voient les autres utilisateurs. Vous pouvez personnaliser de nombreuses parties de l'interface utilisateur (IU), dont les actions à inclure dans le ruban, la manière dont les champs sont placés dans Raccourcis ou dans Récapitulatifs, et les éléments de menu à inclure dans le volet de navigation.

> [!NOTE]  
> Vous pouvez également personnaliser des pages à l'aide du [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Pour apprendre comment fonctionne la personnalisation entre deux clients, voir [Aperçu de la personnalisation](ui-personalization-overview.md).
 
## <a name="how-to-personalize-your-workspace"></a>Comment personnaliser votre espace de travail
Vous effectuez la plus grande partie du travail de personnalisation à l'aide de la fonctionnalité **Personnaliser**, à laquelle vous pouvez accéder depuis pratiquement tous les types de pages, en procédant comme suit :

1.  Ouvrez la page à personnaliser.
2.  En haut à gauche, sélectionnez l'icône de menu **Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis sélectionnez l'une des options de personnalisation.

Il existe aussi des modifications de base de l'interface utilisateur, comme ajuster la taille d'une fenêtre ou élargir des colonnes, que vous pouvez effectuer directement dans la page, en dehors de l'option **Personnaliser**.

## <a name="general-information"></a>Informations générales
Il est bon de garder les éléments suivants à l'esprit lors de la personnalisation de l'interface utilisateur : 

-   Vous pouvez enregistrer plusieurs personnalisations de la même page en fonction des différents points d'accès à la page. Par exemple, la fenêtre Commandes vente peut être personnalisée de manière à être différente lorsqu'elle est ouverte depuis la fenêtre Fiche client que lorsqu'elle est ouverte à partir du Tableau de bord Préparateur de commandes vente. Le point à partir duquel vous accédez à la page à personnaliser est enregistré dans cette personnalisation de page spécifique. Par conséquent, il peut y avoir plusieurs enregistrements de personnalisation de page dans la base de données, comme vous pouvez le voir dans la fenêtre **Supprimer la personnalisation utilisateur**.

-   L'application peut être configurée de sorte à afficher et masquer des éléments de l'interface utilisateur (par exemple des champs, des organisateurs, et des récapitulatifs) en fonction de votre licence ou de vos autorisations. Vous ne pouvez afficher et personnaliser que les champs d'éléments pour lesquels vous êtes autorisé.

## <a name="customize-ribbons"></a>Personnaliser les rubans
Le ruban vous permet d'accéder à plusieurs actions. En personnalisant le ruban, vous pouvez l'optimiser pour vos processus et préférences de travail. Par exemple, si vous utilisez fréquemment la fenêtre **Axes analytiques**, vous pouvez ajouter l'action **Axes analytiques** dans le groupe d'actions **Processus**. Vous pouvez également supprimer les actions que vous n'utilisez jamais pour un meilleur aperçu.  
  
Pour personnaliser les rubans des pages, vous pouvez effectuer les tâches suivantes :  
  
-   Ajouter, renommer ou supprimer des onglets, des groupes, des actions et des menus.  
-   Modifier l'ordre des actions.  
-   Restaurer le ruban afin de rétablir sa configuration par défaut.  
  
### <a name="to-customize-a-ribbon"></a>Pour personnaliser un ruban
1. Ouvrez la page à modifier.
2. En haut à gauche, sélectionnez l'icône de menu **Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Personnaliser le ruban**.

La boîte de dialogue **Organiser les actions dans le ruban** divisée en deux volets. Le volet **Actions disponibles** répertorie toutes les actions que vous pouvez ajouter à la page. Le volet **Afficher les actions dans cet ordre** affiche la structure de toutes les actions actuellement affichées dans la page.

-   Les articles du niveau racine définissent les onglets.

    -   Les articles du second niveau définissent un groupe dans un onglet.

        -   Les articles de troisième niveau définissent un menu d'actions dans un groupe

### <a name="add-a-group"></a>Ajouter un groupe
Sélectionnez l'onglet sous lequel vous souhaitez que se trouve le groupe, puis sélectionnez **Créer un groupe**. Vous ne pouvez pas ajouter de groupe sous un menu.

### <a name="add-a-menu"></a>Ajouter un menu
Sélectionnez le groupe sous lequel vous souhaitez que se trouve le menu, puis sélectionnez **Créer un menu**. Vous ne pouvez ajouter de menu qu'à un groupe ou à un autre menu. 

#### <a name="add-an-action"></a>Ajouter une action
Sélectionnez cette option dans le volet **Actions disponibles**, choisissez **Ajouter** pour l'ajouter au volet **Afficher les actions dans cet ordre**, puis utilisez les boutons **Déplacer vers le haut** et **Déplacer vers le bas** pour la placer où vous le souhaitez.

Vous ne pouvez pas ajouter d'action à un onglet ; uniquement à un groupe ou à un menu.

###  <a name="limitations-and-recommendations"></a>Limitations et recommandations 
N'oubliez pas les restrictions suivantes lorsque vous personnalisez le ruban :  
  
-   Les onglets ou groupes système tels que **Accueil** ou **Nouveau** ne peuvent pas être déplacés ou renommés. La position de certains groupes, tel que **Nouveau document** est fixe.  
-   Les actions ou les groupes ayant une visibilité dynamique ne peuvent pas être ajoutés ni supprimés. 
-   Vous pouvez uniquement créer des menus à l'intérieur des groupes, pas à l'intérieur des onglets.  
-   Vous pouvez imbriquer un menu dans un autre menu, mais ceci n'est pas recommandé.  
-   Si vous voyez un comportement inattendu au niveau des groupes et des actions après avoir personnalisé le ruban, procédez comme suit :  
    
    1.  Videz, mais ne supprimez pas le groupe où le problème survient.  
    2.  Fermez la boîte de dialogue à l'aide du bouton **OK**.  
    3.  Ouvrez à nouveau la boîte de dialogue et ajoutez à nouveau les actions au groupe.  

> [!IMPORTANT]  
>  Toute personnalisation qui modifie le ruban peut affecter les instructions fournies dans l'aide de [!INCLUDE[navnow_md](includes/navnow_md.md)], car les étapes de navigation dans l'aide peuvent faire référence à une autre présentation du ruban.

## <a name="customize-fasttabs"></a>Personnaliser les raccourcis
Les raccourcis vous permettent de répartir les informations sur les pages en groupes simples et faciles à gérer. Vous pouvez personnaliser les raccourcis sur les pages afin qu'ils prennent en charge votre flux de travail. Par exemple, vous pouvez choisir d'afficher moins de raccourcis ou de masquer certains champs dans les raccourcis. Vous pouvez également favoriser les champs les plus importants à inclure dans les en-têtes des raccourcis lorsque ces derniers sont réduits.  

### <a name="to-customize-a-fasttab"></a>Pour personnaliser un raccourci  
  
1.  Ouvrez la page à modifier.
2.  Sélectionnez l'icône de menu **Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Personnaliser cette page**.  
3.  Dans la boîte de dialogue **Personnaliser <Page Name>**, sélectionnez **Raccourcis**.  
  
### <a name="add-move-or-remove-fasttabs"></a>Ajouter, déplacer ou supprimer des raccourcis
La zone **Afficher les raccourcis dans cet ordre** contient les raccourcis actuellement dans la page, et l'ordre dans lequel ils sont affichés. Utilisez les boutons **Ajouter**, **Supprimer**, **Déplacer vers le haut** et **Déplacer vers le bas** pour apporter des modifications.

### <a name="show-and-hide-fields-on-fasttabs"></a>Afficher et masquer des champs de raccourcis
Dans la zone **Afficher les raccourcis dans cet ordre**, sélectionnez le raccourci à modifier, puis choisissez **Personnaliser le raccourci**. Utilisez les boutons pour personnaliser les champs à afficher et leur ordre dans la page.

Définissez l'**Importance** comme suit :
-   Pour afficher le champ dans l'en-tête du raccourci lorsque celui-ci est réduit, définissez cette option sur **Promu**.
- Si vous souhaitez que le champ soit masqué à moins que l'utilisateur ne choisisse l'action **Afficher plus de champs** dans le raccourci, définissez cette option sur **Supplémentaire**.
-   **Standard** est la configuration par défaut ou normale.

### <a name="set-up-field-for-quick-entry"></a>Configurer un champ pour la saisie rapide 
Sélectionnez la case à cocher **Saisie rapide** pour ajouter le champ dans la liste des champs à saisie rapide. Lorsque vous travaillez dans la page et que vous appuyez sur la touche Entrée dans un champ, le pointeur saute au champ suivant défini comme un champ à saisie rapide. 

## <a name="customize-factboxes"></a>Personnaliser les récapitulatifs
Vous utilisez les récapitulatifs pour afficher des informations relatives à l'enregistrement sélectionné dans la liste ou ouvert dans une page de tâche. Vous pouvez sélectionner quels récapitulatifs vous voulez afficher dans le volet Récapitulatif. Il est également possible de personnaliser les récapitulatifs afin de n'afficher que les champs dont vous avez besoin.  
  
### <a name="to-show-or-hide-the-factbox-pane"></a>Pour masquer ou afficher le volet Récapitulatif
Les récapitulatifs se trouvent dans un volet Récapitulatif, que vous pouvez choisir de masquer ou d'afficher pour chaque page. Cela vous permet de masquer facilement plusieurs récapitulatifs sans devoir les supprimer individuellement. 

1.  Ouvrez la page à modifier. 
2.  Sélectionnez l'icône de menu **Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Récapitulatifs**. Une coche indique que le volet Récapitulatif est affiché.  

### <a name="to-customize-the-factbox-pane"></a>Pour personnaliser le volet Récapitulatif  
1.  Ouvrez la page à modifier. 
2.  Sélectionnez l'icône de menu **Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Récapitulatifs**.  
    
### <a name="add-a-factbox"></a>Ajouter un récapitulatif  
  
Sélectionnez le récapitulatif à ajouter au volet Récapitulatif dans la zone **Récapitulatifs disponibles**, puis sélectionnez le bouton **Ajouter**.  
  
### <a name="remove-a-factbox"></a>Supprimer un récapitulatif  
  
Dans la zone **Afficher les récapitulatifs dans cet ordre**, sélectionnez les récapitulatifs, puis le bouton **Supprimer**.   
  
### <a name="change-the-order-of-the-factboxes"></a>Modifier l'ordre des récapitulatifs  
  
Dans la zone **Afficher les récapitulatifs dans cet ordre**, sélectionnez le récapitulatif à déplacer, puis cliquez sur **Déplacer vers le haut** ou **Déplacer vers le bas** jusqu'à ce que le récapitulatif se trouve à l'emplacement voulu.  
  
### <a name="change-the-fields-in-a-factbox"></a>Modifier les champs dans un récapitulatif  
  
1.  Dans la zone **Afficher les récapitulatifs dans cet ordre**, sélectionnez le récapitulatif, puis le bouton **Personnaliser la section**.  
  
2.   La zone **Champs disponibles** répertorie tous les champs proposés. La zone **Champs affichés** affiche tous les champs qui sont actuellement affichés dans le récapitulatif. Utilisez les boutons pour ajouter, supprimer et déplacer des champs.   


## <a name="customize-columns-in-a-list-or-on-document-lines"></a>Personnaliser les colonnes dans une liste ou des lignes document
Pour obtenir un meilleur aperçu des informations dont vous avez besoin, vous pouvez personnaliser les pages de liste et les pages de fiche en ajoutant ou supprimant des colonnes dans les grilles, en réorganisant les colonnes et en ajoutant un volet Figer.  
  
### <a name="to-add-remove-and-arrange-columns"></a>Pour ajouter, supprimer et réorganiser les colonnes  
  
1.  Vous pouvez ajouter, supprimer ou réorganiser les colonnes de deux manières :

    -   Sélectionnez l'icône de menu **Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Choisir les colonnes**.
    -   Cliquez avec le bouton droit sur un en-tête de colonne, puis sélectionnez **Choisir les colonnes**.

2.  Dans la boîte de dialogue **Choisir les colonnes à afficher dans la liste**, le volet **Colonnes disponibles** contient des colonnes masquées. Le volet **Afficher colonnes dans cet ordre** indique les colonnes affichées. Utilisez les boutons **Ajouter** et **Supprimer** pour déplacer les colonnes d'un champ vers l'autre. Utilisez les boutons **Déplacer vers le haut** et **Déplacer vers le bas** pour positionner les colonnes. 

>[!TIP]
>Sélectionnez la case à cocher **Saisie rapide** pour ajouter le champ dans la liste des champs à saisie rapide. Lorsque vous travaillez dans la page et que vous appuyez sur la touche Entrée dans un champ, le pointeur saute au champ suivant défini comme un champ à saisie rapide. 

### <a name="to-set-the-freeze-pane"></a>Pour définir le volet Figer
Une liste peut comporter de nombreuses colonnes, ce qui peut vous forcer à les faire défiler horizontalement pour les afficher toutes. Il peut y avoir des colonnes que vous souhaitez toujours voir, même pendant le défilement. Pour ce faire, vous pouvez ajouter un volet Figer vertical pour empêcher le défilement de certaines colonnes. Cela fait en sorte que seules les colonnes moins importantes bougent lorsque vous faites défiler la page.

Pour définir le volet Figer, sélectionnez la colonne après laquelle vous souhaitez que le volet Figer commence, puis choisissez **Ajouter le volet Figer**.

## <a name="customizing-the-navigation-pane"></a>Personnalisation du volet de navigation
Le volet de navigation affiche un menu de liens vers plusieurs pages de liste. Les liens sont rassemblés sous des boutons au niveau racine. 

### <a name="to-customize-the-navigation-pane"></a>Pour personnaliser le volet de navigation  
  
Sélectionnez l'icône de menu **Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Personnaliser Volet de navigation**.  
  
### <a name="rename-or-rearrange-buttons-in-the-navigation-pane"></a>Renommer ou réorganiser les boutons du volet de navigation  
Dans la boîte de dialogue **Personnaliser Volet de navigation**, dans le volet de gauche, sélectionnez le bouton que vous souhaitez déplacer, renommer ou supprimer, puis choisissez le bouton approprié au milieu de la fenêtre.

Vous ne pouvez pas déplacer, renommer ou supprimer le bouton **Accueil**. Le bouton **Départements** peut être supprimé du volet de navigation, mais il ne peut pas être renommé ou déplacé. 
  
### <a name="add-a-new-menu-button"></a>Ajouter un nouveau bouton de menu 
Vous pouvez créer un bouton au niveau de la racine, puis ajouter un menu de liens sous ce bouton pour ouvrir plusieurs pages.

1. Dans la boîte de dialogue **Personnaliser Volet de navigation**, choisissez **Nouveau**, puis tapez un nom dans le champ **Nom**.
2.  Cliquez sur le bouton **OK**.

Vous pouvez ajouter des liens au bouton.  
  
### <a name="add-a-link-to-a-button"></a>Ajouter un lien à un bouton   
Si vous êtes autorisé à afficher une liste, telle qu'une liste de commandes vente, vous pouvez ajouter un lien vers la liste à partir d'un bouton de votre volet de navigation.  
  
1.  Dans la boîte de dialogue **Personnaliser Volet de navigation**, dans le champ **Boutons du volet de navigation**, sélectionnez le menu auquel vous souhaitez ajouter le lien.  
  
2.  Cliquez sur le bouton **Ajouter**.  
  
3.  Déplacez-vous jusqu'au lien que vous voulez ajouter, puis choisissez le bouton **OK**.  
> [!TIP]
> Si vous trouvez un lien dans les pages **Départements**, vous pouvez également l'ajouter au volet de navigation. Pour plus d'informations, reportez-vous à la section Ajout d'un lien de Départements vers votre tableau de bord.  
  
### <a name="move-or-copy-a-link-from-one-button-to-another"></a>Déplacer ou copier un lien d'un bouton vers un autre  
  
1.  Dans la boîte de dialogue **Personnaliser Volet de navigation**, dans le champ **Boutons du volet de navigation**, sélectionnez le menu dans lequel le lien apparaît.  
  
2.  Dans le volet **Listes**, sélectionnez le lien que vous voulez déplacer, puis choisissez **Déplacer vers** ou **Copier vers**  
  
3.  Sélectionnez le bouton de navigation auquel vous voulez ajouter le lien, puis choisissez le bouton **OK**.  
  
### <a name="rearrange-the-order-of-a-links-under-a-button"></a>Réorganiser l'ordre des liens sous un bouton  
  
1.  Dans le volet **Listes**, sélectionnez le lien que vous souhaitez déplacer.  
  
2.  Utilisez les boutons **Déplacer vers le haut** et **Déplacer vers le bas** pour positionner le lien.

## <a name="adding-department-links-to-the-role-center"></a>Ajouter des liens département au tableau de bord
Vous avez la possibilité d'ajouter le lien d'une page **Départements** à votre Tableau de bord pour y accéder facilement. L'endroit où vous pouvez placer le lien dans le tableau de bord dépend la catégorie du lien dans la page **Départements**.

Le tableau suivant décrit les types de liens de chaque catégorie disponibles dans les pages **Départements** ainsi que l'emplacement de votre Tableau de bord où vous pouvez les ajouter.  
  
|**Catégorie**|**Indique**|**Ajouter un lien vers**|  
|------------------|------------------|---------------------|  
|Listes|Pages de liste|Bouton **Accueil** du volet de navigation|  
|Tâches|Pages de tâche, traitements par lots, feuilles de calcul, feuilles|Onglet **Actions** dans le ruban|  
|États et analyse|Fenêtres d'état, de traitement par lots et matricielles|Onglet **Rapports** dans le ruban|  
|Documents|Documents tels que factures et rappels|**Rapports** dans le ruban|  
|Archives/historique|Documents validés/terminés, registres|Bouton **Accueil** du volet de navigation|  
|Administration|Fenêtres de paramétrage|Onglet **Actions** dans le ruban|  
  
### <a name="to-copy-department-links-to-your-role-center"></a>Pour copier des liens département vers votre Tableau de bord  
  
1.  Ouvrez la page **Départements**.  
  
2.  Cliquez avec le bouton droit sur le lien, puis sélectionnez l'une des options suivantes (seule une de ces options est disponible).  
  
    |**Sélectionner**|**Pour ajouter le lien vers**|  
    |----------------|----------------------------|  
    |**Ajouter au volet de navigation**|Le bouton **Accueil** du volet de navigation de votre tableau de bord.|  
    |**Ajouter aux actions dans le ruban Tableau de bord**|Menu **Actions** sur le ruban de votre tableau de bord|  
    |**Ajouter aux états dans le ruban Tableau de bord**|Menu **États** sur le ruban de votre tableau de bord|  
  
3.  Confirmez le message qui s'affiche.  
  
 Le nouveau lien figure maintenant dans le menu auquel vous l'avez ajouté. Vous pouvez toutefois déplacer ce lien vers un autre emplacement du menu. Par exemple, si vous avez ajouté un lien au volet de navigation, il figurera dans le menu **Accueil**, mais vous pouvez le déplacer vers un autre menu du volet de navigation. Pour plus d'informations, voir la section Personnaliser le volet de navigation. 

## <a name="adding-charts-to-role-centers-and-list-pages"></a>Ajouter des graphiques à des Tableaux de bord et des pages de liste
En cas d'informations complexes, vous pouvez afficher une représentation visuelle des données de manière à mieux voir les tendances et faciliter la prise de décisions. Par exemple, vous pouvez contrôler les soldes par compte en banque pour votre société dans un graphique. Le volet Graphique vous permet d'afficher les données d'une liste dans les types de page suivants :  
  
-   Dans votre tableau de bord, où vous pouvez sélectionner un des graphiques génériques prédéfinis.  
  
-   Dans une page de liste, où vous pouvez afficher une liste sous forme de graphique.  
  
### <a name="to-add-a-generic-chart-to-your-role-center"></a>Pour ajouter un graphique générique à votre Tableau de bord  
  
1.  Dans votre tableau de bord, sélectionnez l'icône de menu **Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Personnaliser cette page**.  
  
2.  Dans la fenêtre **Personnaliser le Tableau de bord**, dans le champ **Sections disponibles**, sélectionnez **Partie de diagramme**, puis choisissez **Ajouter**.  
  
3.  Utilisez les boutons **Déplacer vers le haut**, **Déplacer vers le bas**, **Déplacer vers la gauche** et **Déplacer vers la droite** pour positionner la Partie de diagramme dans votre Tableau de bord.  
  
4.  Sélectionnez le composant graphique, puis **Personnaliser la section**.  
  
5.  Dans la fenêtre **Personnaliser la section**, sélectionnez le graphique prédéfini que vous voulez afficher, puis choisissez le bouton **OK**.  
  
### <a name="to-view-a-list-as-a-chart"></a>Pour afficher une liste sous forme de graphique  
  
1.  Dans la page de liste, sélectionnez l'action **Afficher sous forme de graphique**.  
  
2.  Sélectionnez une mesure et une dimension pour créer un graphique personnalisé. Pour afficher des informations supplémentaires, sélectionnez une dimension secondaire. Par exemple, pour créer un simple graphique à barres, sélectionnez une dimension sur l'axe des abscisses (X) puis sélectionnez la dimension **Comptage d'axes analytiques** sur l'axe des ordonnées (Y).  
  
> [!NOTE]  
>  Par défaut, le volet graphique est masqué parce qu'il risque de ralentir l'application. Affichez le graphique uniquement lorsque les informations sont nécessaires.  
    
## <a name="handling-external-files-and-automation-objects"></a>Traiter les fichiers externes et les objets d'automatisation
Lorsque [!INCLUDE[navnow_md](includes/navnow_md.md)] reçoit un fichier externe, une boîte de dialogue s'affiche. En plus de sélectionner la façon de gérer le fichier, vous pouvez décider comment traiter ce type de fichier à sa prochaine réception.  
  
Lorsque [!INCLUDE[navnow_md](includes/navnow_md.md)] doit exécuter un objet d'automatisation, une boîte de dialogue s'affiche. Vous pouvez décider si ce type d'objet doit toujours ou jamais pouvoir être exécuté.  
  
### <a name="to-specify-how-to-handle-external-files"></a>Pour spécifier comment gérer les fichiers externes  
  
1.  Lorsque la boîte de dialogue s'affiche, désactivez la case à cocher **Toujours demander avant d'ouvrir ce type de fichier** si vous souhaitez que [!INCLUDE[navnow_md](includes/navnow_md.md)] se souvienne de l'option sélectionnée à l'étape 2. La prochaine fois que ce type de fichier sera traité, la boîte de dialogue n'apparaîtra pas et le fichier sera traité comme spécifié à l'étape 2.  
  
     Sinon, activez la case à cocher **Toujours demander avant d'ouvrir ce type de fichier** afin d'afficher toujours la boîte de dialogue lorsque ce type de fichier est reçu.  
  
2.  Sélectionnez **Ouvrir**, **Enregistrer** ou **Annuler**. Le fichier est traité en fonction de votre sélection.  
  
### <a name="to-specify-how-to-handle-automation-objects"></a>Pour spécifier comment gérer les objets d'automatisation  
  
Lorsque la boîte de dialogue s'affiche, cochez la case **Toujours autoriser** si vous souhaitez que [!INCLUDE[navnow_md](includes/navnow_md.md)] exécute toujours ce type d'objet d'automatisation. La prochaine fois que le type de l'objet d'automatisation devra s'exécuter, la boîte de dialogue n'apparaîtra pas, et l'objet d'automatisation s'exécutera directement.  
  
Sinon, activez la case à cocher **Jamais autoriser**. La prochaine fois que le type de l'objet d'automatisation doit s'exécuter, la boîte de dialogue n'apparaîtra pas, et l'objet d'automatisation ne fonctionnera pas.  

## <a name="CancelPersonalization"></a>Annuler la personnalisation
Annuler la personnalisation peut être divisé en deux catégories :

-   l'annulation des modifications que vous avez apportées à l'aide de la fonctionnalité **Personnaliser** ;
-   l'annulation des modifications de base de l'interface utilisateur. 

### <a name="cancel-customization"></a>Annuler la personnalisation
Si vous voulez annuler toutes les personnalisations de l'interface utilisateur que vous avez effectuées pour une page dans votre connexion utilisateur actuelle ou depuis la dernière annulation des personnalisations de l'interface utilisateur, vous pouvez utiliser la fenêtre **Supprimer la personnalisation utilisateur**. La disposition de la page pour laquelle vous supprimez votre personnalisation est alors réinitialisée à la configuration par défaut pour votre profil.  
  
Si vous souhaitez seulement annuler une personnalisation de l'interface utilisateur que vous avez créée pour une zone spécifique d'interface utilisateur sur une page(par ex. le ruban), vous pouvez utiliser le bouton **Rétablir les valeurs par défaut** dans la fenêtre **Personnaliser**. La présentation de la zone d'interface utilisateur spécifique sur cette page est alors réinitialisée à la configuration par défaut pour votre profil.  
  
#### <a name="to-cancel-all-ui-customization-that-you-have-made-to-a-page"></a>Pour annuler toutes les personnalisations de l'interface utilisateur que vous avez créées pour une page  
  
1.  Dans la zone **Rechercher**, entrez **Supprimer la personnalisation utilisateur**, puis sélectionnez le lien associé.  
  
2.  Sélectionnez la page pour laquelle vous souhaitez annuler la personnalisation de l'interface utilisateur, puis, sous l'onglet de **Accueil**, dans le groupe **Affichage**, sélectionnez **Supprimer**.  
  
> [!NOTE]  
>  Toutes les personnalisations de l'interface utilisateur de la page que vous avez effectuées dans votre connexion utilisateur actuelle, ou depuis la dernière fois que vous avez utilisé la fenêtre **Supprimer la personnalisation utilisateur** sont annulées. La disposition de la page est réinitialisée à la configuration par défaut pour votre profil, telle que configurée par l'administrateur ou installée avec Microsoft Dynamics NAV.  
  
#### <a name="to-cancel-ui-customization-that-you-have-made-to-a-ui-area-on-a-page"></a>Pour annuler toutes les personnalisations de l'interface utilisateur que vous avez créées sur une zone d'interface utilisateur d'une page  
  
1.  Dans la page où vous avez personnalisé une zone d'interface utilisateur, par exemple le ruban, sélectionnez l'icône de menu **Application** menu ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis sélectionnez **Personnaliser <UI area>**.  
  
2.  Au bas de la fenêtre **Personnaliser**, choisissez le bouton **Rétablir les valeurs par défaut**.  
  
> [!NOTE]  
>  Toutes les personnalisations de la zone d'interface utilisateur que vous avez effectuées pour la page dans votre connexion utilisateur actuelle, ou depuis la dernière fois que vous avez utilisé le bouton **Rétablir les valeurs par défaut** sont annulées. La disposition de la zone d'interface utilisateur est réinitialisée à la configuration par défaut pour votre profil, telle que configurée par l'administrateur ou installée avec Microsoft Dynamics NAV.

### <a name="cancel-basic-ui-changes"></a>Annuler les modifications de base de l'interface utilisateur
Vous pouvez annuler les modifications de base de l'interface utilisateur en ouvrant la fenêtre **Réinitialiser les paramètres spécifiés par l'utilisateur** de votre Tableau de bord.  
  
Les modifications de base de l'interface utilisateur incluent des éléments comme :
 -  Modifier la taille et la position d'une fenêtre.
 -  Modifier la largeur des colonnes
 -  Modifier la hauteur des en-têtes de colonne.
 -  Trier des colonnes dans une liste.
 -  Afficher des listes sous forme de graphique.
 -  Spécifier comment traiter les fichiers externes et les objets d'automatisation  
 
#### <a name="to-cancel-basic-ui-changes"></a>Pour annuler les modifications de base de l'interface utilisateur
  
1.  Accédez à votre Tableau de bord.  
  
     Dans le menu**Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Réinitialiser les paramètres spécifiés par l'utilisateur**.  
  
2.  Cliquez sur le bouton **Réinitialiser les paramètres de l'interface utilisateur**. Sinon, choisissez le bouton **Réinitialiser tout** pour annuler également vos décisions concernant le traitement des fichiers et des objets d'automatisation.  
  
 Toutes les modifications de base de l'interface utilisateur que vous avez apportées dans votre connexion utilisateur actuelle à [!INCLUDE[navnow_md](includes/navnow_md.md)], ou depuis la dernière fois que vous avez utilisé le bouton **Réinitialiser les paramètres de l'interface utilisateur**, sont annulées. L'interface utilisateur est réinitialisée sur sa configuration par défaut pour votre profil.  
  
#### <a name="to-cancel-your-decision-for-running-or-saving-external-files"></a>Pour annuler votre décision d'exécuter ou enregistrer des fichiers externes  
  
1.  Accédez à votre Tableau de bord.  
  
     Dans le menu**Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Réinitialiser les paramètres spécifiés par l'utilisateur**.  
  
2.  Cliquez sur le bouton **Réinitialiser la décision de traitement des fichiers**. Sinon, choisissez le bouton **Réinitialiser tout** pour annuler également vos modifications d'affichage et vos décisions concernant le traitement des fichiers et des objets d'automatisation.  
  
 Toutes les décisions pour la gestion par défaut des types de fichier que vous avez prises dans votre connexion utilisateur actuelle, ou depuis la dernière fois que vous avez choisi le bouton **Accès au fichier client**, sont annulées et réinitialisées en fonction de la configuration par défaut de votre profil. La prochaine fois que [!INCLUDE[navnow_md](includes/navnow_md.md)] recevra un fichier externe de n'importe quel type, une boîte de dialogue vous sera présentée avec les options **Enregistrer**, **Exécuter** et **Annuler**  
  
### <a name="to-cancel-your-decision-for-handling-automation-objects"></a>Pour annuler votre décision de traiter les objets d'automatisation  
  
1.  Accédez à votre Tableau de bord.  
  
     Dans le menu**Application** ![bouton de menu Application dans la barre de menu](media/applicationmenuicon.png "ApplicationMenuIcon"), sélectionnez **Personnaliser**, puis **Réinitialiser les paramètres spécifiés par l'utilisateur**.  
  
2.  Cliquez sur le bouton **Réinitialiser les décisions d'automatisation**. Sinon, choisissez le bouton **Réinitialiser tout** pour annuler également vos modifications d'affichage et vos décisions concernant l'exécution ou l'enregistrement de fichiers externes.  
  
 Toutes les décisions concernant l'exécution d'objets d'automatisation que vous avez prises dans votre connexion utilisateur actuelle, ou depuis la dernière fois que vous avez choisi le bouton **Réinitialiser les décisions d'automatisation**, sont annulées. Le comportement de traitement de fichier est réinitialisé à la configuration par défaut pour votre profil. La prochaine fois que [!INCLUDE[navnow_md](includes/navnow_md.md)] doit exécuter un objet d'automatisation de n'importe quel type, une boîte de dialogue avec les options **Toujours autoriser** et **Jamais autoriser** vous sera présentée.    

<!--Use the following table to get more information about customizing the different elements of the UI.

| To | See |
| --- | --- |
| Change which actions to show on the ribbon and how the actions are grouped. |[How to: Customize FastTabs](purchasing-how-record-purchases.md) |
|Change which FastTabs to show and which fields to include on the FastTabs.|[How to: Request Quotes](purchasing-how-request-quotes.md)|
|Add, remove, or arrange columns in a list or document-lines that represent fields in the underlying tables. |[ How to: Add or Remove Columns in a List or on Document Lines](purchasing-how-purchase-products-sale.md) |
| Rename or rearrange buttons, create a new menu button, add a link to a menu, or rearrange the order of a menu. |[ How to: Customize the Navigation Pane](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Add a link from a department page to your Role Center. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Add a chart to your Role Center or to a list page.|[How to: Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
| Unod personalization that you have made to your user interface, either for a specific area on a page, such as a ribbon, or for the whole page.|[How to: Cancel Personalization](ui-customization-cancel.md)|
-->


## <a name="see-also"></a>Voir aussi
[Personnalisation de votre espace de travail dans le client Web Dynamics](ui-personalization-user.md)  
[Aperçu de la personnalisation](ui-personalization-overview.md)  



