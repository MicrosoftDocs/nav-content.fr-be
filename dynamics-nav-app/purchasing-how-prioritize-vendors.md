---
title: "Procédure : octroyer une priorité à des fournisseurs"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 3b89bf07e1e9d1839b6c86a01111e936fb62c9f3
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-prioritize-vendors"></a>Procédure : octroyer une priorité à des fournisseurs
Dynamics NAV peut proposer différents paiements aux fournisseurs, par exemple les paiements arrivant à échéance ou les paiements donnant lieu à un escompte. Pour plus d'informations, reportez vous à [Procédure : proposer des paiements fournisseur](payables-how-suggest-vendor-payments.md).

Tout d'abord, vous devez attribuer une priorité à vos fournisseurs en leur affectant des numéros.

## <a name="to-prioritize-vendors"></a>Pour octroyer une priorité à des fournisseurs
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Fournisseurs**, puis sélectionnez le lien connexe.
2. Sélectionnez le fournisseur approprié, puis sélectionnez **Modifier**.
3. Dans le champ **Priorité**, entrez un numéro.

Dynamics NAV donne le degré de priorité le plus élevé au chiffre le plus bas (excepté 0). Ainsi, si vous utilisez 1, 2 et 3, le chiffre 1 a le degré de priorité le plus élevé.

Si vous ne souhaitez pas attribuer de priorité à un fournisseur, laissez le champ **Priorité** blanc. Par la suite, lorsque vous utilisez la fonction de proposition de paiements, ce fournisseur est répertorié après tous les fournisseurs possédant un numéro prioritaire. Vous pouvez saisir autant de niveaux de priorité que nécessaire.

## <a name="see-also"></a>Voir aussi
[Configuration des procédures achat](purchasing-setup-purchasing.md)  
[Gestion des comptes fournisseur](payables-manage-payables.md)

