---
title: TVA belge
description: "Les améliorations belges de la fonction de déclaration de TVA vous permettent d'imprimer des détails sur les transactions TVA."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: fd7b0932f9e6e42dc43aed52382b4cfef7a98056
ms.contentlocale: fr-be
ms.lasthandoff: 10/26/2017

---
# <a name="belgian-vat"></a>TVA belge
[!INCLUDE[navnow](../../includes/navnow_md.md)] ../../ inclut pour la Belgique des améliorations de la fonction de déclaration de TVA vous permettant d'imprimer des détails sur les transactions TVA. Vous devez envoyer les états suivants aux autorités fiscales belges :  

-   Déclaration mensuelle/trimestrielle - Cet état permet de créer des déclarations de TVA mensuelles ou trimestrielles, en fonction des revenus de votre société.  

-   Listing TVA annuel (sur papier/disquette) - Cet état permet de déclarer annuellement tous les montants facturés pour les biens et les services à toutes les sociétés belges avec un numéro de TVA enregistré.  

-   Listing TVA-VIES (sur papier/disquette) - Cet état permet de déclarer les ventes de marchandises à d'autres pays.  

Vous êtes également tenu de fournir un relevé imprimé détaillant les transactions TVA aux autorités fiscales belges. Pour plus d'informations, voir Déclaration TVA.  

## <a name="non-deductible-vat"></a>TVA non déductible  
 En Belgique, la TVA peut être entièrement ou partiellement déductible. Des dépenses comme les frais de représentation ou les achats de voitures ne sont que partiellement déductibles et la transaction doit spécifier quel pourcentage de la TVA est non déductible. Par exemple, vous créez un compte général pour les immobilisations comme les voitures, et un autre compte pour les frais de représentation. Pour chaque compte, vous spécifiez quel pourcentage de la TVA déclarée est non déductible en définissant le champ Pourcentage TVA non déductible. Ensuite, lorsque vous validez une transaction, la TVA déductible sera validée sur le compte TVA correspondant, et la TVA non déductible sera ajoutée au montant de base et validée sur le même compte que les immobilisations corporelles et incorporelles.  

 Pour les immobilisations, la TVA non déductible est amortie simplement comme le coût d'acquisition de base de l'immobilisation. Vous devez paramétrer des groupes comptabilisation immobilisation distincts pour chaque pourcentage de TVA non déductible, étant donné que chaque groupe comptabilisation immobilisation est validé sur un compte général où le champ Pourcentage TVA non déductible spécifie quel pourcentage de TVA doit être validé sur le même compte que l'immobilisation.  

 Si vous sélectionnez le champ TVA non déductible comprise dans une ligne déclaration TVA, la TVA non déductible est incluse dans le montant TVA. L'état **Calculer et valider décl. TVA** ajoute la partie non déductible de ce montant aux champs **Montant TVA non déductible** et **Montant TVA devise origine non déductible** dans les écritures TVA résultantes.  

## <a name="see-also"></a>Voir aussi  
 [Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)   
 [Comment imprimer des déclarations de TVA périodiques](how-to-print-periodic-vat-reports.md)   
 [Comment configurer la TVA non déductible](how-to-set-up-non-deductible-vat.md)

