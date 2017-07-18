---
title: "Procédure : enregistrer de nouveaux produits"
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
ms.openlocfilehash: df84a4d3e15035cd956c7612a12069844f5601d2
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-products"></a>Procédure : enregistrer de nouveaux produits

Les produits sont la base de votre activité, les biens ou les services que vous commercialisez. Chaque produit doit être enregistré en tant que fiche article.

**Remarque** : dans Dynamics NAV, un produit est désigné par le terme « article ».

Les fiches article contiennent les informations nécessaires à l'achat, le stockage, la vente, la livraison et la comptabilisation des biens.

La fiche article peut être de type Stock ou Service pour spécifier si le produit est une unité physique ou une unité temporelle de main-d'œuvre. Mis à part certains champs liés à l'aspect physique d'un article, tous les champs d'une fiche article fonctionnent de la même manière pour les articles de stock et les services. Pour plus d'informations sur la vente d'un article , reportez-vous à [Procédure : vendre des produits](sales-how-sell-products.md) ou à [Procédure : facturer les ventes](sales-how-invoice-sales.md).

**Remarque** : si des modèles article existent pour différents types d'articles, une fenêtre s'affiche automatiquement lorsque vous créez une nouvelle fiche article à partir de laquelle vous pouvez sélectionner un modèle article approprié. Si un seul modèle article existe, les nouvelles fiches article utiliseront toujours ce modèle.

## <a name="to-create-a-new-item-card"></a>Pour créer une fiche article
1. Sur la page d'accueil, sélectionnez l'action **Articles** pour ouvrir la liste des article existants.  
2. Dans la fenêtre **Articles**, sélectionnez l'action **Nouveau**.

    Si un seul modèle article existe, une nouvelle fiche article avec certains champs renseignés à l'aide des informations provenant du modèle s'ouvre.
3. Dans la fenêtre **Sélectionnez un modèle pour un nouvel article**, sélectionnez le modèle que vous souhaitez utiliser pour la nouvelle fiche article.
4. Cliquez sur le bouton **OK**. Une nouvelle fiche article avec certains champs renseignés à l'aide des informations provenant du modèle s'ouvre.
5. Continuez à renseigner ou modifier les champs de la fiche article selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

Sur le raccourci **Prix vente**, vous pouvez afficher les prix spécifiques ou les remises accordées pour l'article si certains critères sont réunis, par exemple le client, la quantité minimum commande ou la date de fin. Chaque ligne représente un prix spécial ou une remise ligne. Chaque colonne représente un critère qui doit s'appliquer pour garantir le prix spécial que vous saisissez dans le champ **Prix** ou la remise ligne que vous saisissez dans le champ **% remise ligne**. Pour plus d'informations, reportez-vous à [Enregistrement des prix de vente, des remises et des accords sur les paiements](sales-how-record-sales-price-discount-payment-agreements.md).

L'article est désormais enregistré, et la fiche article est prête à être utilisée sur les documents d'achat et de vente.

Si vous souhaitez utiliser cette fiche article comme modèle lorsque vous créez de nouvelles fiches article, enregistrez-la comme modèle. Pour plus d'informations, reportez-vous à la section suivantes.

## <a name="to-save-the-item-card-as-a-template"></a>Pour enregistrer la fiche article en tant que modèle
1. Dans la fenêtre **Fiche article**, sélectionnez l'action **Sauvegarder comme modèle**. La fenêtre **Modèle article** s'ouvre et affiche la fiche article comme modèle.
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Pour réutiliser les axes analytiques dans les modèles **, sélectionnez l'action **Axes analytiques**. La fenêtre **Modèles axe** s'ouvre et affiche tous les codes axe qui sont définis pour l'article.
4. Modifiez ou entrez les codes axe s'appliquant aux nouvelles fiches article créées à l'aide du modèle.
5. Lorsque vous avez terminé le nouveau modèle article, cliquez sur le bouton **OK**.

Le modèle article est ajouté à la liste des modèles article. Vous pouvez ainsi l'utiliser pour créer des fiches article.

## <a name="see-also"></a>Voir aussi
  [Gestion du stock](inventory-manage-inventory.md)  
  [Gestion des achats](purchasing-manage-purchasing.md)  
  [Gestion des ventes](sales-manage-sales.md)

