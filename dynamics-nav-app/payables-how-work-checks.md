---
title: "Procédure : utilisation des chèques"
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
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a>Procédure : utilisation des chèques
Dynamics NAV prend en charge l'émission électronique et manuelle de chèques. Ces deux méthodes utilisent la feuille paiement pour émettre des chèques aux fournisseurs. Vous pouvez également annuler des chèques et afficher les écritures comptables chèque.

La procédure d'émission de chèques propose des paiements, crée des écritures comptables et imprime les chèques informatiques.

Votre imprimante doit être correctement configurée pour les formulaires chèque, et vous devez définir la mise en page de chèque à utiliser. Pour plus d'informations, reportez-vous à [Procédure : définir les mises en page de chèques](finance-setup-how-define-check-layouts.md)

## <a name="to-issue-checks"></a>Pour émettre des chèques
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuilles paiement**, puis sélectionnez le lien connexe.
2. Remplissez la feuille avec les paiements appropriés, par exemple à l'aide de la fonction Proposer paiements fournisseur. Pour plus d'informations, reportez vous à [Procédure : proposer des paiements fournisseur](payables-how-suggest-vendor-payments.md).
3. Dans le champ **Mode émission paiement** des lignes feuille pour le paiement que vous souhaitez effectuer avec des chèques, sélectionnez l'une des options suivantes :

 - **Informatique** : sélectionnez cette option si vous souhaitez imprimer un chèque du montant de la ligne feuille paiement. Vous devez imprimer les chèques avant de pouvoir valider les lignes feuille. Vous pouvez uniquement sélectionner **Informatique** si le **Type compte contrepartie** ou le **Type compte** est **Compte bancaire**.

 - **Manuel** : sélectionnez cette option si vous avez créé un chèque manuellement et que vous souhaitez créer une écriture comptable chèque correspondante de ce montant. Si vous utilisez cette option, vous ne pouvez pas imprimer de chèque à partir de Dynamics NAV. Vous pouvez uniquement sélectionner **Manuel** si le **Type compte contrepartie** ou le **Type compte** est **Compte bancaire**.

    **Remarque** : vous devez imprimer les chèques informatiques avant de valider les lignes feuille correspondantes.
4. Dans le cas de chèques informatiques, sélectionnez **Imprimer chèque**.
5. Dans la fenêtre **Chèque**, renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
6. Cliquez sur le bouton **Imprimer**.

**Remarque** : si vous souhaitez imprimer des chèques en plusieurs devises sur des comptes bancaires différents, vous devez exécuter le traitement par lots **Imprimer chèque** pour chacune de ces devises et préciser le compte bancaire concerné.

## <a name="to-cancel-printed-checks-that-are-not-posted"></a>Pour annuler des chèques imprimés qui ne sont pas validés
Vous pouvez annuler des chèques non validés après leur impression par l'intermédiaire de l'action **Annuler chèque** de la fenêtre **Feuille paiement**.
1. Dans la fenêtre **Feuille paiement**, sélectionnez **Annuler chèque**, puis sélectionnez les chèques à annuler.

## <a name="to-void-checks"></a>Pour annuler des chèques
Lorsque des paiements par chèque ont été validés, vous pouvez uniquement annuler des chèques à partir des écritures comptables banque ainsi obtenues.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Comptes bancaires**, puis sélectionnez le lien connexe.
2. Sélectionnez le compte bancaire approprié, sélectionnez l'action **Modifier**, puis l'action **Écritures comptables chèque**.
3. Dans la fenêtre **Écritures comptables chèque**, sélectionnez l'action **Annuler chèque**.
4. Cochez la case **Annuler chèque uniquement**.
5. Cliquez sur le bouton **OK**.

## <a name="see-also"></a>Voir aussi
[Gestion des comptes fournisseur](payables-manage-payables.md)  
[Configuration des opérations bancaires](bank-setup-banking.md)  

