---
title: "Procédure : configurer un indicateur coloré sur des piles"
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
ms.openlocfilehash: 04272431b01c0ab398618d9878b90d73e6324abe
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---
    
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a>Procédure : configurer un indicateur coloré sur des piles
Vous pouvez configurer des piles qui apparaissent sur la page **Accueil** afin d'inclure un indicateur qui change de couleur en fonction des valeurs de données dans les piles. 

L'indicateur apparait sous forme d'une barre de couleur le long de la bordure supérieure de la mosaïque Pile. Il offre un signal visuel du statut de l'activité de la pile, ce qui peut indiquer des conditions favorables ou défavorables pour inviter l'utilisateur à prendre des mesures. Par exemple, si une pile affiche les factures vente en cours, vous pouvez définir l'indicateur pour qu'il apparaisse vert (favorable) lorsque le nombre total des factures vente en cours est inférieur à 10, et apparaisse rouge (défavorable) lorsque le total est supérieur à 20.

Dans la fenêtre **Paramètres pile**, vous configurez des indicateurs pour toutes les piles disponibles dans la base de données de la société.

Pour configurer l'indicateur, vous pouvez spécifier jusqu'à deux valeurs de seuil qui définissent trois plages de valeurs de données (basse, moyenne et haute) à laquelle vous pouvez appliquer une couleur différente (ou un style différent).

## <a name="to-set-up-colored-indicators-on-cues"></a>Pour paramétrer des indicateurs colorés sur des piles
1. Sous **Activités** sur votre page **Accueil**, sélectionnez **Paramétrer piles**.  
La fenêtre **Paramètres pile** s'affiche. La fenêtre répertorie les indicateurs actuellement paramétrés sur des piles.
2. Pour modifier un indicateur, modifiez les champs et modifiez, par exemple, les valeurs pour des seuils différents.  

Le tableau suivant répertorie les couleurs correspondant aux options des champs **Style bas de gamme**, **Style milieu de gamme** et **Style haut de gamme**.

|Option|Couleur|
|------|-----|
|**Aucun**|Aucune couleur (même couleur que la mosaïque Pile|
|**Favorable**|Vert|
|**Défavorable**|Rouge|
|**Ambigu**|Jaune|
|**Subordonné**|Gris|

## <a name="see-also"></a>Voir aussi
[Utiliser Dynamics NAV](ui-work-product.md)


