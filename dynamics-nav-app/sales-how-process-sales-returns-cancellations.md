---
title: "Procédure : traiter les retours ou annulations de ventes"
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
ms.openlocfilehash: 92b65379f2ec633712a2b2c0f06615c6de61cc6e
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-sales-returns-or-cancellations"></a>Procédure : traiter les retours ou annulations de ventes
Si votre client souhaite retourner ou obtenir un remboursement pour des articles, ou encore annuler des services, que vous lui avez vendus et pour lesquels vous avez reçu un paiement, vous devez créer et valider un avoir vente qui indique la modification demandée. Pour inclure les informations de facture vente correctes, vous pouvez créer l'avoir vente à partir de la facture vente enregistrée ou utiliser la fonction de copie.

Outre la facture vente validée d'origine, vous pouvez lettrer l'avoir vente à d'autres documents vente, par exemple une autre facture vente validée, parce que le client renvoie également des articles livrés avec cette facture.

Un retour ou un remboursement peut en effet se rapporter uniquement à certains des articles ou des services figurant sur la facture vente initiale. Dans ce cas, vous devez modifier les informations des lignes de l'avoir vente. Lors de la validation de l'avoir vente, les documents vente affectés par la modification sont contrepassés et un paiement de remboursement peut être créé pour le client.

Vous pouvez envoyer l'avoir vente validé au client pour confirmer le retour ou l'annulation et communiquer que la valeur associée sera remboursée, par exemple lorsque les articles sont renvoyés.

## <a name="to-create-a-sales-credit-memo-from-a-posted-sales-invoice"></a>Pour créer un avoir vente à partir d'une facture vente validée
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Factures vente enregistrées**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Factures vente enregistrées**, sélectionnez la facture vente validée que vous souhaitez contrepasser, puis sélectionnez l'action **Créer un avoir correctif**.

    La plupart des champs de l'en-tête de l'avoir vente sont renseignés avec les informations de la facture vente validée. Vous pouvez modifier tous les champs, par exemple avec de nouvelles informations qui reflètent l'accord de retour.
3. Modifiez les informations des lignes en fonction de l'accord, par exemple le nombre d'articles retournés ou du montant à rembourser.
4. Sélectionnez l'action **Lettrer écritures**.
5. Dans la fenêtre **Lettrer écritures client**, sélectionnez la ligne contenant le document vente validé auquel vous souhaitez lettrer l'avoir vente, puis sélectionnez l'action **ID lettrage**.

    Le numéro de l'avoir vente est inséré dans le champ **ID lettrage**.  
6. Dans le champ **Montant à lettrer**, entrez le montant à lettrer s'il est inférieur au montant initial.

    Au bas de la fenêtre **Lettrer écritures client**, vous pouvez afficher le montant total à lettrer pour contrepasser toutes les écritures concernées, à savoir lorsque la valeur du champ **Solde** est égale à zéro.  
7. Cliquez sur le bouton **OK**. Lors de la validation de l'avoir vente, il doit être lettré avec les documents vente validés spécifiés.

    Lorsque vous avez créé ou modifié les lignes avoir vente nécessaires et qu'un ou plusieurs lettrages sont spécifiées, vous pouvez procéder à la validation de l'avoir vente.
8. Sélectionnez l'action **Valider et envoyer**.

La boîte de dialogue **Valider et envoyer la confirmation** s'ouvre et indique le mode d'envoi par défaut du client. Vous pouvez modifier le mode d'envoi en cliquant sur le bouton de recherche pour le champ **Envoyer le document à**. Pour plus d'informations, reportez vous à [Procédure : configurer des profils d'envoi de documents](sales-how-setup-document-send-profiles.md).

Les documents vente validés auxquels vous avez lettré l'avoir sont à présent contrepassés, et un remboursement peut être créé pour le client. L'avoir vente est supprimé et remplacé par un nouveau document dans la liste des avoirs vente validés.

## <a name="to-create-a-sales-credit-memo-from-scratch"></a>Pour créer un avoir vente à partir de zéro
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Factures vente enregistrées**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau** pour ouvrir un nouvel avoir vente vierge.
3. Dans le champ **Client**, entrez le nom d'un client existant.
4. Sélectionnez l'action **Copier document**.
5. Dans la fenêtre **Extraire document vente**, dans le champ **Type document**, sélectionnez **Facture enregistrée**.
6. Sélectionnez le champ **N° document** pour ouvrir la fenêtre **Factures vente enregistrées**, puis sélectionnez la facture vente validée qui contient les lignes que vous souhaitez contrepasser.
7. Activez la case à cocher **Recalculer lignes** si vous souhaitez que les lignes facture vente validées copiées soient mises à jour avec les modifications apportées au prix article et au coût unitaire depuis la validation de la facture.
8. Cliquez sur le bouton **OK**. Les lignes facture copiées sont insérées dans l'avoir vente.
9. Remplissez l'avoir vente en vous reportant à la section « Pour créer un avoir vente à partir d'une facture vente validée » de cette rubrique.

## <a name="see-also"></a>Voir aussi  
[Gestion des ventes](sales-manage-sales.md)  
[Configuration des ventes](sales-setup-sales.md)  
[Procédure : envoyer des documents par e-mail](ui-how-send-documents-email.md)  
[Utiliser Dynamics NAV](ui-work-product.md)
