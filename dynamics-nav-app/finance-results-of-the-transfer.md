---
title: "Résultats du transfert"
description: "Cette rubrique décrit ce qui se produit après le transfert des écritures comptables vers les écritures de coûts."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: general ledger, transfer, cost entries
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 05da79520b5568a8b8e63f10efce9c8b3c5395b8
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="results-of-transferring-general-ledger-entries-to-cost-entries"></a>Résultats du transfert des écritures comptables vers les écritures de coûts
Lors du transfert des écritures comptables vers les écritures de coûts, [!INCLUDE[d365fin](includes/d365fin_md.md)] crée des connexions dans les écritures dans les tables **Écriture comptable**, **Écriture de coûts** et **Registre de coûts** pour assurer le suivi des connexions entre les écritures de coûts et les écritures comptables.  

## <a name="general-ledger-entries"></a>Écritures comptables  
Pour chaque écriture comptable transférée vers la comptabilité analytique, [!INCLUDE[d365fin](includes/d365fin_md.md)] renseigne le champ **N° écriture**  

## <a name="cost-entries"></a>Écritures de coûts  
Pour chaque écriture de coûts, [!INCLUDE[d365fin](includes/d365fin_md.md)] garde le numéro de l'écriture comptable correspondante dans le champ **N° séquence compta.** de la table **Écriture de coûts**.  

Pour les écritures de coûts combinées, [!INCLUDE[d365fin](includes/d365fin_md.md)] garde le numéro de la dernière écriture comptable, à savoir l'écriture avec le numéro le plus élevé.  

Le champ **Compte général** de la table **Écriture de coûts** contient le numéro du compte général, d'où provient l'écriture de coûts.  

Pour les écritures de coûts uniques, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfère le texte de validation depuis l'écriture comptable vers le champ de texte **Description**. Pour les écritures combinées, le champ de texte indique que ces écritures sont transférées en tant qu'écritures combinées. Par exemple, pour une écriture combinée pour octobre 2013, le texte peut être **Écritures combinées, octobre 2013**.  

## <a name="cost-register"></a>Registre de coûts  
Dans la table **Registre de coûts**, [!INCLUDE[d365fin](includes/d365fin_md.md)] crée une écriture à l'aide du transfert source depuis la comptabilité. L'écriture enregistre le premier et le dernier numéros des écritures comptables transférées, outre le premier et le dernier numéros des écritures de coûts créées.  

## <a name="see-also"></a>Voir aussi  
[Comment transférer les écritures comptables vers les écritures de coûts](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md)   
[Critères de transfert des écritures comptables vers les écritures de coûts](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md)   
[Transfert automatique et écritures combinées](finance-automatic-transfer-combined-entries.md)   
[Transfert et validation des écritures de coûts](finance-transfer-and-post-cost-entries.md)  

