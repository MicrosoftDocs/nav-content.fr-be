---
title: "Procédure : enregistrer les prix vente et les remises"
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
ms.openlocfilehash: 2d6438108fb2c36bb6f0d44efddc053bd628d068
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-sales-prices-and-discounts"></a>Procédure : enregistrer les prix vente et les remises
Vous devez définir les différents accords de prix et de remise qui s'appliquent lors de la vente à différents clients de sorte que les valeurs et règles convenues s'appliquent aux documents vente crées pour les clients.

En ce qui concerne les prix, un prix de vente spécial peut être inséré sur les lignes vente s'il existe une certaine combinaison de client, d'article, de quantité minimum, d'unité de mesure ou de date de début/date de fin.

En ce qui concerne les remises, vous pouvez définir et utiliser deux types de remises vente :

|Type de remise |Description |
|--------------|------------|
|**Remise ligne vente**|Une remise sous forme de montant insérée sur les lignes vente s'il existe une certaine combinaison de client, d'article, de quantité minimum, d'unité de mesure ou de date de début/date de fin. Cela fonctionne de la même manière que pour les prix de vente.|
|**Remise facture**|Une remise en pourcentage qui est soustraite du total du document si la valeur de toutes les lignes d'un document vente dépasse un montant minimal donné.|

Dans la mesure où les prix de vente et les remises ligne vente sont basés sur une combinaison article/client, vous pouvez également mettre en œuvre cette configuration à partir de la fiche article de l'article auquel les règles et valeurs s'appliquent.

## <a name="to-set-up-a-sales-price-for-a-customer"></a>Pour définir un prix de vente pour un client
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Clients**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche client appropriée, puis sélectionnez l'action **Prix**.

    Le champ **Type vente** est prérempli avec la valeur **Client** et le champ **Code vente** est prérempli avec le numéro du client.
3. Renseignez les champs de la ligne selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
4. Renseignez une ligne pour chaque combinaison qui accorde un prix de vente spécial au client.

## <a name="to-set-up-a-sales-line-discount-for-a-customer"></a>Pour définir une remise ligne vente pour un client
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Clients**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche client appropriée, puis sélectionnez l'action **Remises ligne**.

    Le champ **Type vente** est prérempli avec la valeur **Client** et le champ **Code vente** est prérempli avec le numéro du client.
3.  Renseignez les champs de la ligne selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
4. Renseignez une ligne pour chaque combinaison qui accorde une remise ligne vente au client.

## <a name="to-set-up-an-invoice-discount-for-a-customer"></a>Pour configurer une remise facture pour un client
Une fois que vous avez décidé des clients pouvant faire l'objet de remises facture, entrez le code remise facture dans les fiches client et configurez les conditions de chaque code.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Clients**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche client d'un client pouvant faire l'objet de remises facture.
3. Dans le champ **Code remise facture**, sélectionnez un code pour les conditions de remise facture appropriées à utiliser pour calculer les remises facture pour le client.

    **Remarque** : les codes remise facture sont représentés par les fiches client existantes. Cela vous permet d'affecter rapidement les conditions de remise facture aux clients en sélectionnant le nom d'un autre client qui bénéficie des mêmes conditions.

    Configurez de nouvelles conditions de remise facture vente.
4. Dans la fenêtre **Fiche client**, sélectionnez l'action **Remises facture**. La fenêtre **Remises facture client** s'ouvre.
5. Dans le champ **Code devise**, indiquez le code d'une devise à laquelle s'appliquent les conditions de remise facture. Laissez le champ vierge si vous souhaitez configurer des conditions de remise facture en USD.
6. Dans le champ **Montant minimum**, entrez le montant minimal qu'une facture doit présenter pour faire l'objet de la remise.
7. Dans le champ **% remise**, entrez la remise facture sous la forme d'un pourcentage du montant de la facture.
8. Répétez les étapes 5 à 7 pour chaque devise pour laquelle le client recevra une remise facture différente.

La remise facture est désormais configurée et affectée au client concerné. Lorsque vous sélectionnez le code client dans le champ **Code remise facture** dans d'autres fiches client, la même remise facture est affecté à ces clients.

## <a name="see-also"></a>Voir aussi  
[Configuration des ventes](sales-setup-sales.md)  
[Gestion des ventes](sales-manage-sales.md)
