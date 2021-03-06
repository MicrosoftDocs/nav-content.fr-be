---
title: "Détails de conception - Lot pour lot"
description: "Découvrez comment utiliser la méthode lot pour lot pour déterminer la quantité de commande en fonction de la demande."
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
ms.openlocfilehash: 039afd9dd6f7e4c608b17229f5b438c23ba3624b
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-lot-for-lot"></a>Détails de conception : lot pour lot
La méthode lot pour lot est la plus souple, parce que le système réagit uniquement à la demande réelle, de plus il agit sur une demande anticipée à partir de commandes de prévision et de commandes ouvertes, puis détermine la quantité commande en fonction de la demande. La méthode lot pour lot visé cible les articles A et B pour lesquels le stock peut être accepté mais doit être évité.  
  
Par certains côtés, la méthode lot pour lot ressemble à la méthode de commande, mais elle a une approche générique des articles ; elle peut accepter des quantités en stock, et elle groupe une demande et un approvisionnement correspondants dans des intervalles de planification définis par l'utilisateur.  
  
L'intervalle de planification est défini dans le champ **Intervalle de planification**. Le système travaille avec un intervalle de planification minimum d'un jour, car il s'agit de la plus petite unité de temps des événements de demande et d'approvisionnement dans le système (même si, dans la pratique, l'unité de temps des ordres de fabrication et des besoins de composants peuvent être des secondes).  
  
L'intervalle de planification fixe également des limites lorsque un ordre de fabrication existant doit être replanifié pour répondre à une demande donnée. Si l'approvisionnement se trouve dans l'intervalle de planification, il est replanifié en entrée ou en sortie pour répondre à la demande. Sinon, s'il a lieu précédemment, il provoque une accumulation de stock inutile et doit être annulé. S'il se trouve plus tard, une commande approvisionnement est créée à la place.  
  
Avec cette méthode, il est également possible de définir un stock de sécurité pour compenser les fluctuations possibles de l'approvisionnement, ou répondre à une demande soudaine.  
  
Étant donné que la quantité de commande approvisionnement est basée sur la demande réelle, il peut sembler raisonnable d'utiliser les modificateurs de commande : arrondir la quantité commandée pour répondre à un multiple spécifié de la commande (ou unité d'achat), augmenter la commande à une quantité de commande minimale spécifiée, ou réduire la quantité à la quantité maximale spécifiée (et ainsi créer deux ou plusieurs approvisionnements pour répondre à la quantité nécessaire totale).  
  
## <a name="see-also"></a>Voir aussi  
[Détails de conception : méthodes de réapprovisionnement](design-details-reordering-policies.md)   
[Détails de conception : paramètres de planification](design-details-planning-parameters.md)   
[Détails de conception : gestion des méthodes de réapprovisionnement](design-details-handling-reordering-policies.md)   
[Détails de conception : planification de l'approvisionnement](design-details-supply-planning.md)
