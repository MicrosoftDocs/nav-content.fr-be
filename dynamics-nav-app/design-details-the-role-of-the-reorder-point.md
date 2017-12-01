---
title: "Détails de conception - Le rôle du point de commande"
description: "Cette rubrique met l'accent sur l'importance de définir un point de commande, afin de déterminer quand commander plus de stock."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8035a670077e53981e9c366d22bdb20df06d8c1b
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-role-of-the-reorder-point"></a>Détails de conception : Le rôle du point de commande
En plus de l'équilibrage général de la demande et de l'approvisionnement, le système de planification doit également contrôler les niveaux de stock des articles affectés pour respecter les méthodes de réapprovisionnement définies.  
  
Un point de commande représente la demande lors d'un délai. Lorsque le stock prévisionnel passe en dessous du niveau de stock défini par le point de commande, il est temps de commander une plus grande quantité. Par ailleurs, le stock doit diminuer progressivement et probablement atteindre zéro (ou le niveau de stock de sécurité), jusqu'à ce que le réapprovisionnement arrive.  
  
Par conséquent, le système de planification suggère une commande approvisionnement planifiée en aval au moment où le stock projeté passe sous le point de commande.  
  
Le point de commande indique un certain niveau de stock. Cependant, les niveaux de stock peuvent changer de façon significative au cours de l'intervalle de planification et, par conséquent, le système de planification doit constamment surveiller le stock disponible projeté.  
  
## <a name="see-also"></a>Voir aussi  
[Détails de conception : méthodes de réapprovisionnement](design-details-reordering-policies.md)   
[Détails de conception : paramètres de planification](design-details-planning-parameters.md)   
[Détails de conception : gestion des méthodes de réapprovisionnement](design-details-handling-reordering-policies.md)   
[Détails de conception : planification de l'approvisionnement](design-details-supply-planning.md)
