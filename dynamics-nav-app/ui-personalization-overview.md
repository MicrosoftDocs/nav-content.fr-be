---
title: Personnalisation de votre espace de travail - Vue d'ensemble
description: "Découvrez comment personnaliser l'interface utilisateur pour l'adapter à votre méthode de travail."
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 04334d3bb50b37b9643b848ca4f59b015f03ad04
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace---overview"></a>Personnalisation de votre espace de travail - Vue d'ensemble
Vous pouvez *personnaliser* votre espace de travail pour l'adapter à vos habitudes et préférences en modifiant la disposition des pages afin qu'elles n'affichent que les informations dont vous avez besoin, où vous avez en besoin. Les modifications de personnalisation que vous apportez n'affectent que ce que vous voyez, pas ce que voient les autres utilisateurs.

Vous pouvez personnaliser votre espace de travail à l'aide de [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] et [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Les modifications de personnalisation que vous faites sont également vues dans [!INCLUDE[nav_phone_md](includes/nav_phone_md.md)] et [!INCLUDE[nav_web_md](includes/nav_phone_md.md)].
  
> [!NOTE]  
> L'administrateur dans votre société peut avoir déjà personnalisé votre interface utilisateur par une présentation spécifique au rôle pour tous les utilisateurs qui ont le même profil que vous et qui utilisent le même Tableau de bord. Les personnalisations apportées à votre espace de travail sont enregistrées sous votre compte d'utilisateur. Elles seront donc conservées même si un administrateur déploie un nouvel ensemble de dispositions spécifique à un rôle dans votre société. Pour plus d'informations, voir [Configurer l’interface utilisateur](admin-configure-user-interface.md).

## <a name="comparing-personalization-in-the-dynamics-nav-windows-and-web-clients"></a>Comparer la personnalisation dans les clients Dynamics NAV Windows et web
Selon la page, vous pouvez personnaliser de nombreuses parties de l'interface utilisateur, telles que les champs ou les colonnes qui s'affichent et à quel endroit, les actions incluses dans le ruban, etc. Un grand nombre des choses que vous pouvez faire sont possibles à la fois dans le client Windows et le client web. Le tableau suivant offre une vue d'ensemble des possibilités de personnalisation de chaque client.

|  Personnaliser  ||  Client Windows  |  Client web  |
|---------------|-|------------------|--------------|
|Champs dans les raccourcis||||
||Ajouter, déplacer, supprimer |x|x|
||Afficher dans l'en-tête réduit|x||
||Masquer sous l'action **Afficher plus de champs**|x||
|Listes ou lignes document ||||
||Ajouter, déplacer, supprimer des colonnes  |x|x|
||Ajouter, déplacer, supprimer le volet Figer  |x|x|
|Récapitulatifs|||
||Déplacer, supprimer|x|x|
||Ajouter|x||
||Ajouter, déplacer, supprimer des champs|x|x|
|Piles||||
||Déplacer, supprimer|x|x|
||Ajouter |x||
|Graphiques||||
||Déplacer, supprimer|x|x|
||Ajouter|x| |
|Ruban et actions||x||
|Volet de navigation||x||

Une autre différence est qu'en personnalisant à l'aide du client Windows, vous pouvez avoir différentes versions personnalisées de la même page, selon les différents points d'accès à la page. Par exemple, la page personnalisée **Commandes vente** peut être différente lorsqu'elle est ouverte depuis la page **Fiche client** et lorsqu'elle est ouverte à partir de la page **Préparateur de commandes vente**. Lorsque vous personnalisez une page à l'aide du client web, il n'existe qu'une version personnalisée par page ; ainsi, les modifications apportées seront visibles dans la page indépendamment de l'endroit à partir duquel vous l'ouvrez.

##  <a name="PersonalizationWinWeb"></a>Utilisation de la personnalisation entre le client Dynamics NAV Windows et le client web
Avant de personnaliser des pages, il est important de comprendre comment fonctionne la personnalisation entre le client Windows et le client web. Si vous n'utilisez jamais qu'un des deux, cette information n'est pas très importante. Toutefois, elle a de l'importance si vous commencez à personnaliser des pages en utilisant les deux clients, ou que vous passez de l'utilisation du client Windows à l'utilisation permanente du client web.  

-   Si vous utilisez le client Windows pour personnaliser une page spécifique dès le début, vous verrez également les modifications de personnalisation de la page dans le [!INCLUDE[nav_web_md](includes/nav_web_md.md)].

-   Tant que vous continuerez à utiliser le client Windows pour personnaliser la page, toutes les modifications de personnalisation que vous apporterez s'appliqueront également à la page dans le client web.

-   Toutefois, dès que vous commencerez à personnaliser la page en utilisant le client web, la personnalisation de cette page deviendra distincte entre les deux clients, et vous aurez une version personnalisée pour chaque client. Dans le client web, les personnalisations précédentes de la page sont effacées, ce qui signifie que la page revient à sa disposition initiale, et vous recommencerez à personnaliser la page depuis le début. Les personnalisations précédentes du client Windows sont inchangées.

- À partir de là, vous personnaliserez la page dans le client Windows et le client web indépendamment l'un de l'autre, ce qui implique que la page peut avoir un aspect différent dans chaque client. Les clients pour téléphone et tablette affichent les mêmes personnalisations de page que le client web.  

> [!Tip]  
>Si vous ouvrez la page **Supprimer la personnalisation utilisateur**, vous pouvez voir toutes les pages qui ont été personnalisées par chaque utilisateur. La colonne **Personnalisation héritée** vous indique si la personnalisation a été effectuée dans le client Windows ou le client web. S'il y a une coche dans la colonne, la personnalisation a été effectuée dans le client Windows (ou dans le client web avant [!INCLUDE[navnow_md](includes/navnow_md.md)]).

## <a name="see-also"></a>Voir aussi
[Personnalisation de votre espace de travail dans le client Windows Dynamics NAV](ui-personalization-windows-client.md)  
[Personnalisation de votre espace de travail dans le client web Dynamics NAV](ui-personalization-user.md)  
[Gérer la personnalisation](ui-personalization-manage.md)  
[Personnalisation de Dynamics NAV](ui-customizing-overview.md)  

