---
title: "Procédure : traiter les retours ou annulations d'achats"
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 94067fb3d10975c1db29d2e3f1d5d6373fcbf9f2
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-purchase-returns-or-cancellations"></a>Procédure : traiter les retours ou annulations d'achats
Si vous souhaitez retourner des articles à votre fournisseur ou annuler des services que vous avez achetés, vous pouvez créer et valider un avoir achat qui indique la modification demandée par rapport à la facture achat d'origine. Pour inclure les informations de facture achat correctes, vous pouvez créer l'avoir achat à partir de la facture achat enregistrée ou utiliser la fonction de copie.

Généralement, vous pouvez créer un avoir achat en réaction un avoir que vous a envoyé un fournisseur. L'avoir achat fonctionne comme votre documentation interne du processus d'avoir à des fins comptables.

La modification peut concerner tous les produits figurant sur la facture achat d'origine, ou uniquement certains d'entre eux. Par conséquent, vous pouvez partiellement renvoyer les articles reçus ou demander le remboursement partiel des services reçus. Dans ce cas, vous devez modifier les informations de facture achat copiées.

Outre la facture achat validée d'origine, vous pouvez lettrer l'avoir achat à d'autres documents achat, par exemple une autre facture achat validée, parce que vous renvoyez également des articles livrés avec cette facture.

## <a name="to-create-a-purchase-credit-memo-from-a-posted-purchase-invoice"></a>Pour créer un avoir achat à partir d'une facture achat validée
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Avoirs achat**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Factures achat enregistrées**, sélectionnez la facture achat validée que vous souhaitez contrepasser, puis sélectionnez l'action **Créer un avoir correctif**.

    La plupart des champs de l'en-tête de l'avoir achat sont renseignés avec les informations de la facture achat validée. Vous pouvez modifier tous les champs, par exemple avec de nouvelles informations qui reflètent l'accord de retour.
3. Modifiez les informations des lignes en fonction de l'accord, par exemple le nombre d'articles retournés ou du montant à rembourser.
4. Sélectionnez l'action **Lettrer écritures**.
5. Dans la fenêtre **Lettrer écritures fournisseur**, sélectionnez la ligne contenant le document achat validé auquel vous souhaitez lettrer l'avoir achat, puis sélectionnez l'action **ID lettrage**. Le numéro de l'avoir achat est inséré dans le champ **ID lettrage**.
6. Dans le champ **Montant à lettrer**, entrez le montant à lettrer s'il est inférieur au montant initial.

    Au bas de la fenêtre **Lettrer écritures fournisseur**, vous pouvez afficher le montant total à lettrer pour contrepasser toutes les écritures concernées, à savoir lorsque la valeur du champ **Solde** est égale à zéro.
7. Cliquez sur le bouton **OK**. Lorsque vous validez l'avoir achat, il est lettré avec les documents achat validés spécifiés.

    Lorsque vous avez créé ou modifié les lignes avoir achat nécessaires et qu'une ou plusieurs applications sont spécifiées, vous pouvez procéder à la validation de l'avoir achat.
8. Sélectionnez l'action **Valider**.

Les factures achat validées auxquelles vous appliquez l'avoir sont à présent contrepassées. Si vous avez déjà payé la facture initiale, le fournisseur doit maintenant rembourser le paiement en votre faveur. Si l'avoir est uniquement pour une partie du produit dans la facture initiale, vous pouvez payer uniquement le montant restant de la facture achat d'origine pour la clôturer.

L'avoir achat est supprimé et remplacé par un nouveau document dans la liste des avoirs achat validés.

## <a name="to-create-a-purchase-credit-memo-from-scratch"></a>Pour créer un avoir achat à partir de zéro
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Factures achat enregistrées**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau** pour ouvrir un nouvel avoir achat vierge.
3. Dans le champ **Fournisseur**, entrez le nom d'un fournisseur existant.
4. Sélectionnez l'action **Copier document**.
5. Dans la fenêtre **Extraire document achat**, dans le champ **Type document**, sélectionnez **Facture enregistrée**.
6. Sélectionnez le champ **N° document** pour ouvrir la fenêtre **Factures achat enregistrées**, puis sélectionnez la facture achat validée qui contient les lignes que vous souhaitez contrepasser.
7. Activez la case à cocher **Recalculer lignes** si vous souhaitez que les lignes facture achat validées copiées soient mises à jour avec les modifications apportées au prix article et au coût unitaire depuis la validation de la facture.
8. Cliquez sur le bouton **OK**. Les lignes facture copiées sont insérées dans l'avoir achat.
9. Remplissez l'avoir achat en vous reportant à la section « Pour créer un avoir achat à partir d'une facture achat validée » de cette rubrique.

## <a name="see-also"></a>Voir aussi
[Gestion des achats](purchasing-manage-purchasing.md)  
[Procédure : enregistrer des achats](purchasing-how-record-purchases.md)  

