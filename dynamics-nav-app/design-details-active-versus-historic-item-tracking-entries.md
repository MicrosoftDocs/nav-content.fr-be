---
title: "Détails de conception - Comparaison entre écritures traçabilité actives et historiques"
description: "Lorsque des parties d'une quantité de ligne document sont validées, seule cette quantité particulière est transférée vers les écritures comptables article et ses numéros de suivi. Toutefois, vous voudrez accéder à toutes les informations de traçabilité pertinentes directement à partir de la ligne document actif. C'est-à-dire, non seulement vous voudrez visualiser les écritures relatives à la quantité restante, mais vous voudrez également des informations sur les unités validées. Lorsque vous consultez ou modifiez la fenêtre **Lignes traçabilité**, le contenu collectif du tableau **Spécification traçabilité** (T336) et du tableau **Ecriture réservation** (T337) est présenté dans une version temporaire de T336. Ceci garantit que les données de suivi article historiques et actives sont accessibles en même temps."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 315b5317c2ac3e2cd6a56bd243e30d4e3445a6ec
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-active-versus-historic-item-tracking-entries"></a>Détails de conception : comparaison entre écritures traçabilité actives et historiques
Lorsque des parties d'une quantité de ligne document sont validées, seule cette quantité particulière est transférée vers les écritures comptables article et ses numéros de suivi. Toutefois, vous voudrez accéder à toutes les informations de traçabilité pertinentes directement à partir de la ligne document actif. C'est-à-dire, non seulement vous voudrez visualiser les écritures relatives à la quantité restante, mais vous voudrez également des informations sur les unités validées. Lorsque vous consultez ou modifiez la fenêtre **Item Tracking Lines**, le contenu collectif du tableau **Tracking Specification** (T336) et du tableau **Reservation Entry** (T337) est présenté dans une version temporaire de T336. Ceci garantit que les données de suivi article historiques et actives sont accessibles en même temps.  

 Le tableau suivant montre la manière dont T336 et T337 sont utilisés dans un scénario achat. Les chiffres en gras représentent les valeurs entrées manuellement par l'utilisateur dans la fenêtre **Lignes traçabilité**.  

 Étape 1 : Créez une ligne commande achat de sept pièces avec les numéros traçabilité.  

||**Quantité (base)**|**Qté à traiter**|**Qté à facturer (base)**|**Quantité traitée (base)**|**Quantité facturée (base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**T337**|7|0|0|0|0|  
|**T336**|0|0|0|0|0|  

 Étape 2 : Recevez quatre pièces.  

||**Quantité (base)**|**Qté à traiter**|**Qté à facturer (base)**|**Quantité traitée (base)**|**Quantité facturée (base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Lignes traçabilité** fenêtre|7|**4**|**0**|0|0|  
|**T337**|3|0|0|0|0|  
|**T336**|4|0|0|4|0|  

 Étape 3 : Recevez deux pièces et facturez deux pièces.  

||**Quantité (base)**|**Qté à traiter**|**Qté à facturer (base)**|**Quantité traitée (base)**|**Quantité facturée (base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Lignes traçabilité** fenêtre|7|**2**|**2**|4|0|  
|**T337**|0|0|0|0|0|  
|**T336**|6|0|0|6|2|  

 Étape 4 : Recevez une pièce.  

||**Quantité (base)**|**Qté à traiter**|**Qté à facturer (base)**|**Quantité traitée (base)**|**Quantité facturée (base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Lignes traçabilité** fenêtre|7|**1**|**0**|6|2|  
|**T336**|7|0|0|7|2|  

 Facturez 5 pièces.  

||**Quantité (base)**|**Qté à traiter**|**Qté à facturer (base)**|**Quantité traitée (base)**|**Quantité facturée (base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Lignes traçabilité** fenêtre|7|0|**5**|7|2|  
|**T336**|7|0|0|7|7|  

## <a name="see-also"></a>Voir aussi  
 [Détails de conception : traçabilité](design-details-item-tracking.md)   
 [Détails de conception : fenêtre Lignes traçabilité](design-details-item-tracking-lines-window.md)

