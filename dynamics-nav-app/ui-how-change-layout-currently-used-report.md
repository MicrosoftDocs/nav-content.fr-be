---
title: "Procédure : Modification de la présentation actuellement utilisée sur un rapport"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f1411704a7b2a0565d4b23d91e04e271af07659e
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-change-which-layout-is-currently-used-on-a-report"></a>Procédure : Modification de la présentation actuellement utilisée sur un rapport
Un rapport peut être créé avec plus d'une présentation de rapport, que vous pouvez ensuite changer au besoin.

Selon les présentations qui sont disponibles pour un rapport, vous pouvez choisir d'utiliser une présentation de rapport RDLC intégrée, une présentation de rapport Word, ou une présentation personnalisée. Pour plus d'informations sur les présentations de rapport RDLC et Word, les présentations intégrées et personnalisées, et plus encore, reportez-vous à [Gérer la présentation des états](ui-manage-report-layouts.md).

## <a name="to-change-the-layout-that-is-used-on-a-report"></a>Pour modifier la présentation qui est utilisée dans un état
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Sélection présentation état**, puis sélectionnez le lien connexe.  
La fenêtre **Sélection présentation état** répertorie tous les états disponibles pour la société spécifiée dans le champ Société en haut de la fenêtre. Le champ Présentation sélectionnée spécifie la présentation qui est actuellement utilisée sur l'état.
2. Définissez le champ **Société** en haut de la fenêtre sur la société qui inclut le rapport.
3. Pour modifier la présentation utilisée par un état, sur la ligne correspondant à l'état dans la liste, définissez le champ **Présentation sélectionnée** sur l'une des options suivantes :
    - RDLC (intégré), utilise la présentation d'état RDLC intégrée sur l'état.
    - Word (intégré), utilise la présentation d'état Word intégrée sur l'état.
    - Personnalisée, utilise une présentation personnalisée sur l'état.  
    Il est possible de savoir quelles sont les présentations personnalisées disponibles pour l'état dans le récapitulatif Partie présentations état. S'il n'existe aucune présentation personnalisée pour le rapport, alors vous devez d'abord en créer une. Si vous choisissez cette option, rendez-vous à la procédure suivante pour spécifier la présentation personnalisée que vous souhaitez utiliser.
**Remarque** : si vous choisissez **RDLC (intégré)** ou **Word (intégré)** et que vous recevez un message d'erreur indiquant que l'état n'a pas de présentation du type spécifié, vous devez alors choisir une autre option de présentation ou créer une présentation d'état personnalisée du type que vous souhaitez utiliser.

Si vous avez sélectionné une présentation de rapport RDLC ou Word intégrée, aucune action supplémentaire n'est requise et la présentation sera utilisée la prochaine fois que le rapport sera exécuté.

## <a name="to-specify-a-custom-layout-on-a-report"></a>Pour spécifier une présentation personnalisé sur un état
1. Vous spécifiez la présentation personnalisée à utiliser dans l'état à partir de la fenêtre **Présentations état personnalisées**. Si la fenêtre **Présentations état personnalisées** n'est pas ouverte, cliquez sur le bouton de consultation du champ **Description présentation état**.
2. Dans la fenêtre **Présentations état personnalisées**, sélectionnez la ligne de la présentation personnalisée que vous souhaitez utiliser, puis cliquez sur le bouton **OK**.

La fenêtre **Sélection présentation état** s'affiche à nouveau. Le nom de la présentation personnalisée sélectionnée s'affiche dans le champ **Description présentation personnalisée**. La présentation personnalisée sera utilisée la prochaine fois que vous exécuterez l'état.

## <a name="see-also"></a>Voir aussi
[Gérer la présentation des états](ui-manage-report-layouts.md)

