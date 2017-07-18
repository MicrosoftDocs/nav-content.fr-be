---
title: "Procédure : créer des offres"
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
ms.openlocfilehash: e126c755a9121c3a91f3af72f3f1ae14702a4701
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-offers"></a>Procédure : créer des offres
Vous créez un devis pour enregistrer votre proposition à un client pour vendre certains biens selon certaines conditions de livraison et de paiement. Vous pouvez envoyer un devis au client pour communiquer la proposition. Vous pouvez envoyer par e-mail le document en pièce jointe au format PDF. Vous pouvez faire en sorte que le corps du message soit prérempli avec un résumé du devis. Pour plus d'informations, reportez vous à [Procédure : envoyer des documents par e-mail](ui-how-send-documents-email.md).

Lorsque vous négociez avec le client, vous pouvez modifier et renvoyer autant de devis que nécessaire. Lorsque le client accepte le devis, vous convertissez le devis en facture vente ou en commande vente dans laquelle vous traitez la vente. Pour plus d'informations, reportez-vous à [Procédure : facturer des ventes](sales-how-invoice-sales.md) ou à [Procédure : vendre des produits](sales-how-sell-products.md).

Les produits peuvent être des articles en stock et des services. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md). Le processus de devis est identique pour les deux types de produits.

**Remarque** : dans Dynamics NAV, un produit est désigné par le terme « article ».

Vous pouvez remplir les champs relatifs au client sur le devis de deux façons selon que le client est déjà enregistré ou non.

## <a name="to-create-a-sales-quote"></a>Pour créer un devis
1. Sur la page d'accueil, sélectionnez l'action **Devis**.  
2. Dans le champ **Client**, entrez le nom d'un client existant.

    D'autres champs de la fenêtre **Devis** sont désormais renseignés avec les informations standard sur le client sélectionné. Si le client n'est pas enregistré, procédez comme suit :

3. Dans le champ **Client**, entrez le nom du nouveau client.
4. Dans la boîte de dialogue d'enregistrement du nouveau client, cliquez sur le bouton **Oui**.
5. Dans la fenêtre **Sélectionnez un modèle pour un nouveau client**, sélectionnez un modèle sur lequel baser la nouvelle fiche client, puis cliquez sur le bouton **OK**.
6. Une nouvelle fiche client préremplie avec les informations sur le modèle client sélectionné s'ouvre. Le champ **Nom** est prérempli avec le nom du nouveau client que vous avez saisi sur la facture vente.
7. Renseignez les autres champs de la fiche client. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux clients](sales-how-register-new-customers.md).  
8. Lorsque vous avez terminé la fiche client, cliquez sur le bouton **OK** pour revenir à la fenêtre **Devis**.

    Plusieurs champs du devis sont désormais renseignés avec les informations que vous avez spécifiées sur la nouvelle fiche client.
9. Renseignez les champs restants de la fenêtre **Devis**, selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

    Vous êtes maintenant prêt à renseigner les lignes devis avec les articles en stock ou les services que vous voulez proposer au client.

    **Remarque** : si vous avez défini des lignes vente récurrentes pour le client, tel qu'un ordre de réapprovisionnement mensuel, vous pouvez insérer ces lignes sur le devis par l'intermédiaire de l'action **Extraire les lignes vente récurrentes**.
10. Sur le raccourci **Lignes**, dans le champ **N° article**, saisissez le numéro d'un article en stock ou d'un service.
11. Dans le champ **Quantité**, saisissez le nombre d'articles à proposer.

    **Remarque** : pour les articles de type Service, la quantité est une unité de temps, telle que les heures, comme indiqué dans le champ **Code unité** de la ligne.

    Le champ **Montant ligne** est mis à jour pour indiquer la valeur du champ **Prix unitaire** multipliée par la valeur du champ **Quantité**.

    Le prix et les montants ligne sont affichés avec ou sans la Sales Tax en fonction de la valeur que vous avez sélectionnée dans le champ **Prix incluant la Sales Tax** de la fiche client.
12. Dans le champ **% remise ligne**, saisissez un pourcentage si vous souhaitez accorder au client une remise sur le produit. La valeur du champ **Montant ligne** est mise à jour en conséquence.

    **Remarque**: si vous avez défini des prix article spéciaux sur le raccourci **Prix vente et remises ligne vente** dans la fiche client ou article, le prix et le montant de la ligne devis sont automatiquement mis à jour si les critères de prix convenus sont réunis. Pour plus d'informations, reportez-vous à [Enregistrement des prix de vente, des remises et des accords sur les paiements](sales-how-record-sales-price-discount-payment-agreements.md).
13. Pour ajouter un commentaire sur la ligne devis que le client peut afficher dans le devis vente imprimé, saisissez un texte dans le champ **Description** sur une ligne vierge.  
14. Répétez les étapes 10 à 13 pour chaque article que vous souhaitez proposer au client.

    Les totaux sous les lignes sont calculés automatiquement au fur et à mesure que vous créez ou modifiez des lignes.
15. Dans le champ **Montant remise facture**, entrez un montant qui doit être déduit de la valeur indiquée dans le champ **Total TTC**.

    **Remarque**: si vous avez défini des remises facture pour le client, le pourcentage spécifié est automatiquement inséré dans le champ **% remise facture** si les critères sont réunis, et le montant associé est inséré dans le champ **Montant remise facture sans TVA**. Pour plus d'informations, reportez-vous à [Enregistrement des prix de vente, des remises et des accords sur les paiements](sales-how-record-sales-price-discount-payment-agreements.md).
16. Lorsque les lignes devis sont renseignées, sélectionnez l'action **Envoyer par e-mail** ou **Imprimer**.

    Si vous sélectionnez l'action **Envoyer par e-mail**, alors un fichier PDF est automatiquement joint à l'e-mail envoyé au client. Vous pouvez configurer l'e-mail de sorte qu'il contienne un résumé du devis. Pour plus d'informations, reportez vous à [Procédure : envoyer des documents par e-mail](ui-how-send-documents-email.md).
17. Si le client accepte le devis, sélectionnez l'action **Établir facture** ou **Créer commande**.

Le devis est supprimé de la base de données. Une facture vente ou une commande vente basée sur les informations du devis et dans laquelle vous pouvez traiter la vente est créée. Dans le champ **N° devis** de la facture vente ou de la commande vente, vous pouvez visualiser le numéro du devis à partir duquel elle a été réalisée. Pour plus d'informations, reportez-vous à [Procédure : facturer des ventes](sales-how-invoice-sales.md) ou à [Procédure : vendre des produits](sales-how-sell-products.md).

## <a name="see-also"></a>Voir aussi  
[Gestion des ventes](sales-manage-sales.md)  
[Configuration des ventes](sales-setup-sales.md)  
[Procédure : envoyer des documents par e-mail](ui-how-send-documents-email.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

