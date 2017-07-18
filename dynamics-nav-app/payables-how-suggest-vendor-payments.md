---
title: "Procédure : proposer des paiements fournisseur"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 11bfba9f279f6bd84c5d169f6f97fd48759bc6df
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-suggest-vendor-payments"></a>Procédure : proposer des paiements fournisseur
Dans la fenêtre **Feuille paiement**, vous pouvez utiliser une fonction pour proposer des lignes paiement en fonction de vos paramètres, tels que les paiements échus à courte échéance ou les paiements pour lesquels un escompte est disponible.

Pour bénéficier pleinement de la fonction Proposer paiements fournisseur, vous devez d'abord attribuer une priorité à vos fournisseurs. Pour plus d'informations, reportez-vous à [Procédure : octroyer une priorité à des fournisseurs](purchasing-how-prioritize-vendors.md).

Les écritures fournisseur qui ne sont pas marquées **En attente** ne sont pas incluses dans le traitement par lots.  

**Important**: si vous souhaitez profiter d'escomptes et que vous avez saisi un montant disponible, ce montant est d'abord utilisé pour les écritures fournisseur échues et prioritaires, par ordre de priorité, puis pour les écritures fournisseur échues et non prioritaires, et enfin pour les écritures fournisseur ouvertes donnant lieu à un escompte, dans l'ordre des numéros des fournisseurs.

## <a name="to-use-the-suggest-vendor-payments-function"></a>Pour utiliser la fonction Proposer paiements fournisseur
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuilles paiement**, puis sélectionnez le lien connexe.
2. Ouvrez la feuille appropriée, puis sélectionnez l'action **Proposer paiements fournisseur**.
3. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
4. Cliquez sur le bouton **OK**.

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a>Pour insérer la date d'échéance comme date comptabilisation sur les lignes feuille paiement
Lorsque vous utilisez le traitement par lots **Proposer paiements fournisseur** pour créer des lignes de paiement pour vos fournisseurs, vous pouvez remplir deux champs spéciaux pour vous assurer que les lignes générées utilisent la date d'échéance pour calculer la date comptabilisation. Ces champs sont **Calculer la date comptabilisation à partir de la date d'échéance doc. lettrage** et **Décalage date d'échéance doc. lettrage**.

**Important** : vous ne pouvez pas utiliser le champ **Calculer la date comptabilisation à partir de la date d'échéance doc. lettrage** avec le champ **Rechercher les escomptes** ni le champ **Totaliser par fournisseur**. La raison est que si la date comptabilisation est basée sur la date d'échéance, un certain escompte peut ne pas être calculé correctement, parce que la date comptabilisation peut se trouver après la date d'escompte.
Notez également que si la date comptabilisation calculée se trouve dans le passé, la date de comptabilisation est déplacée pour correspondre à la date de travail, et un message d'avertissement s'affiche.

Vous pouvez également créer manuellement des lignes de paiement à l'aide de la date d'échéance pour calculer la date comptabilisation. Une fois que vous avez appliqué les écritures comptables fournisseur, vous pouvez utiliser l'action **Calculer date comptabilisation**. Cela a pour effet de mettre à jour la date comptabilisation de la ligne feuille à la date d'échéance de la facture achat associée. Pour plus d'informations, reportez-vous à [Procédure : Lettrer les achats manuellement](payables-how-apply-purchase-transactions-manually.md).  

**Remarque** : si la facture achat est en retard, la date comptabilisation est définie sur la date de travail et la police de la ligne s'affiche en rouge.

## <a name="see-also"></a>Voir aussi
[Gestion des comptes fournisseur](payables-manage-payables.md)  
[Exécuter des paiements](payables-make-payments.md)  
[Utilisation des feuilles comptabilité](ui-work-general-journals.md)

