---
title: "Procédure : enregistrer les prix achat et les remises"
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
ms.openlocfilehash: f99bb0aeef2c25048b0da3e0476ae2d612bff562
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-record-purchase-prices-and-discounts"></a>Procédure : enregistrer les prix achat et les remises
Vous devez définir les différents accords de prix et de remise qui s'appliquent lors d'achats effectués auprès de plusieurs fournisseurs de sorte que les valeurs et règles convenues s'appliquent aux documents achat créés à l'intention des fournisseurs.

En ce qui concerne les prix, un prix d'achat spécial peut être inséré sur les lignes achat s'il existe une certaine combinaison de fournisseur, d'article, de quantité minimum, d'unité de mesure ou de date de début/date de fin.

En ce qui concerne les remises, vous pouvez définir et utiliser deux types de remises achat :

|Type de remise |Description |
|--------------|------------|
|**Remise ligne achat**|Une remise sous forme de montant insérée sur les lignes achat s'il existe une certaine combinaison de fournisseur, d'article, de quantité minimum, d'unité de mesure ou de date de début/date de fin. Cela fonctionne de la même manière que pour les prix d'achat.|
|**Remise facture**|Une remise en pourcentage qui est soustraite du total du document si la valeur de toutes les lignes d'un document achat dépasse un montant minimal donné.|

Dans la mesure où les remises ligne achat et les prix achat sont basés sur une combinaison article/fournisseur, vous pouvez également effectuer cette configuration à partir de la fiche article dans laquelle sont définies les règles et valeurs. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md).

## <a name="to-set-up-a-special-purchase-price-for-a-vendor"></a>Pour configurer un prix d'achat spécial pour un fournisseur
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Fournisseurs**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche fournisseur appropriée, puis sélectionnez l'action **Prix**.

    Le champ **Type d'achat** est prérempli avec **Fournisseur** et le champ **Code achat** est prérempli avec le numéro du fournisseur.
3. Renseignez les champs de la ligne selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
4. Remplissez une ligne pour chaque combinaison pour laquelle le fournisseur vous accorde une remise ligne achat.

## <a name="to-set-up-a-line-discount-for-a-vendor"></a>Pour configurer une remise ligne pour un fournisseur
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Fournisseurs**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche fournisseur appropriée, puis sélectionnez l'action **Remises ligne**.

    Le champ **Type d'achat** est prérempli avec **Fournisseur** et le champ **Code achat** est prérempli avec le numéro du fournisseur.
3. Renseignez les champs de la ligne selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
4. Remplissez une ligne pour chaque combinaison pour laquelle le fournisseur vous accorde une remise ligne achat.

## <a name="to-set-up-an-invoice-discount-for-a-vendor"></a>Pour configurer une remise facture pour un fournisseur
Une fois que vos fournisseurs vous ont informé des remises facture qu'ils accordent, entrez le code remise facture sur la fiche fournisseur et configurez les conditions pour chaque code.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Fournisseurs**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche fournisseur d'un fournisseur pouvant faire l'objet de remises facture.
3. Dans le champ **Code remise facture**, sélectionnez un code pour les conditions de remise facture appropriées à utiliser pour calculer les remises facture pour le fournisseur.

    **Remarque** : les codes remise facture sont représentés par les fiches fournisseur existantes. Cela vous permet d'affecter rapidement les conditions de remise facture aux fournisseurs en sélectionnant le nom d'autres fournisseurs qui bénéficient des mêmes conditions.

    Configurez de nouvelles conditions de remise facture pour les achats.
4. Dans la fenêtre **Fiche fournisseur**, sélectionnez l'action **Remises facture**. La fenêtre **Remises facture fournisseur** s'ouvre.
5. Dans le champ **Code devise**, indiquez le code d'une devise à laquelle s'appliquent les conditions de remise facture. Laissez le champ vierge si vous souhaitez configurer des conditions de remise facture en USD.
6. Dans le champ **Montant minimum**, entrez le montant minimal qu'une facture doit présenter pour faire l'objet de la remise.
7. Dans le champ **% remise**, entrez la remise facture sous la forme d'un pourcentage du montant de la facture.
8. Répétez les étapes 5 à 7 pour chaque devise pour laquelle le fournisseur recevra une remise facture différente.

La remise facture est désormais configurée et affectée au fournisseur concerné. Lorsque vous sélectionnez le code fournisseur dans le champ **Code remise facture** dans d'autres fiches fournisseur, la même remise facture est affecté à ces fournisseurs.

## <a name="see-also"></a>Voir aussi  
[Configuration des procédures achat](purchasing-setup-purchasing.md)  
[Gestion des achats](purchasing-manage-purchasing.md)

