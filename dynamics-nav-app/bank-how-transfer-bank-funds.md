---
title: "Procédure : Transfert de fonds à la banque"
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f34bef80c64cbad0a0b20d4d021cefbdc5a1cb64
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-transfer-bank-funds"></a>Procédure : Transfert de fonds à la banque
Vous pouvez avoir à transférer un montant d'un compte bancaire à un autre. Pour cela, vous devez valider une transaction dans la feuille comptabilité. La tâche varie selon que les comptes bancaires utilisent la même devise ou des devises différentes.

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a>Pour valider un transfert entre comptes bancaires avec le même code devise
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille comptabilité**, puis sélectionnez le lien connexe.
2. Dans une ligne feuille, renseignez les champs **Date comptabilisation** et **N° document**. .
3. Cliquez sur le champ **Type compte**, sélectionnez le **Compte bancaire**.
4. Dans le champ **N° compte**, sélectionnez la banque à partir de laquelle vous souhaitez transférer les fonds.
5. Dans le champ **Montant**, entrez le total à transférer.
6. Dans le champ **Type compte contrepartie**, sélectionnez **Compte bancaire**.
7. Dans le champ **N° compte contrepartie**, sélectionnez le compte bancaire vers lequel vous souhaitez transférer les fonds.
8. Validez la feuille.

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a>Pour valider des transferts entre comptes bancaires dotés de codes devise différents
Pour transférer des fonds entre des comptes bancaires qui utilisent des devises différentes, vous devez valider deux lignes feuille comptabilité.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille comptabilité**, puis sélectionnez le lien connexe.
2. Créez deux lignes feuille, et renseignez les champs **Date comptabilisation** et **N° document** . .
3. Sur la première ligne feuille, dans le champ **Type**, sélectionnez **Compte bancaire**.
4. Dans le champ **N° compte**, sélectionnez le compte bancaire à partir duquel vous souhaitez transférer les fonds.
5. Dans le champ **Montant**, saisissez le montant dans la devise du compte bancaire. Entrez les montants de crédit précédés du signe moins. Entrez les montants de débit sans signe moins.
6. Dans le champ **Type compte contrepartie**, sélectionnez **Compte bancaire**.
7. Dans le champ **N° compte contrepartie**, sélectionnez le compte bancaire vers lequel vous souhaitez transférer les fonds.
8. Sur la seconde ligne feuille, dans le champ **Type**, sélectionnez **Compte bancaire**.
9. Dans le champ **N° compte**, sélectionnez le compte bancaire vers lequel vous souhaitez transférer les fonds.
10. Dans le champ **Montant**, saisissez le montant dans la devise du compte bancaire. Entrez les montants de crédit précédés du signe moins. Entrez les montants de débit sans signe moins.
11. Dans le champ **Type compte contrepartie**, sélectionnez **Compte bancaire**.  
12. Dans le champ **N° compte contrepartie**, sélectionnez le compte bancaire à partir duquel vous souhaitez transférer les fonds.

    **Remarque** : si les taux de change utilisés dans la feuille sont différents des taux de change qui s'affichent dans la fenêtre **Taux de change devise**, entrez alors une troisième ligne pour les pertes ou gains liés au taux de change. Entrez **Compte général** dans le champ **Type compte**. Entrez le numéro de compte général pour les gains ou les pertes liés au taux de change dans le champ **N° compte** . Saisissez les gains ou les pertes liés au taux de change dans le champ **Montant** avec ou sans signe moins pour les crédits et les débits, respectivement.
13. Validez la feuille.

## <a name="see-also"></a>Voir aussi  
[Gérer les comptes bancaires](bank-manage-bank-accounts.md)  
[Configuration des opérations bancaires](bank-setup-banking.md)  
[Utilisation des feuilles comptabilité](ui-work-general-journals.md)
