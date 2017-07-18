---
title: "Procédure : utiliser des articles non stockés"
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 2b49d95904732dcf091fd060a96006fdcb477ec1
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-nonstock-items"></a>Procédure : utiliser des articles non stockés
Vous pouvez proposer certains articles à vos clients pour leur rendre service, que vous ne souhaitez pas conserver en stock tant que vous ne commencez pas à les commercialiser. Lorsque vous souhaitez commencer à maintenir de tels articles en stock, vous pouvez les convertir en fiches article normales de deux façons.

- Depuis une fiche article non stocké, créez une nouvelle fiche article basée sur un modèle.
- Depuis une ligne commande vente avec un champ **Article** vide, sélectionnez un article non stocké. Lorsque vous validez la vente, une fiche article est automatiquement créée pour l'article non stocké.

**Remarque** : vous ne pouvez pas sélectionner d'article non stocké à partir de la fenêtre **Facture vente**. Vous pouvez sélectionner un article non stocké à partir de la fenêtre **Devis**, mais l'article non stocké ne sera pas converti en un article normal lorsque vous utilisez la fonction **Créer commande**.

Un article non stocké a généralement le numéro d'article du fournisseur qui le fournit. Pour activer la conversion d'une fiche article non stocké en une fiche article normale, vous devez tout d'abord configurer comment la numérotation de l'article fournisseur est convertie dans votre propre numérotation d'article.   

## <a name="to-create-a-nonstock-item"></a>Pour créer un article non stocké
Les fiches article non stocké ont moins d'informations que les fiches article normales, car vous ne les utilisez que pour proposer des devis ainsi que pour d'autres procédures. Pour cette raison, elles doivent être converties en fiches article normales, avant que vous puissiez valider les transactions commerciales pour elles.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Articles non stockés**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau**.
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

## <a name="to-set-up-how-nonstock-item-numbers-are-converted-to-your-own-numbering"></a>Pour configurer comment les numéros d'article non stocké sont convertis en votre propre numérotation  
Pour activer la conversion d'une fiche article non stocké en une fiche article normale, vous devez tout d'abord configurer comment la numérotation de l'article fournisseur est convertie dans votre propre format de numérotation d'article.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Paramètres art. non stockés**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins.

## <a name="to-convert-a-nonstock-item-to-a-normal-item"></a>Pour convertir un article non stocké en un article normal
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Articles non stockés**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche pour un article non stocké que vous pouvez convertir en un article normal.
3. Dans la fenêtre **Fiche article non stocké**, sélectionnez l'action **Créer un article**.

Une nouvelle fiche article pré-remplie avec les informations de l'article non stocké ainsi qu'un modèle d'article pertinent sont créés. Vous pouvez ensuite remplir ou modifier les champs sur la nouvelle fiche article, le cas échéant. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md).

## <a name="to-sell-a-nonstock-item-and-convert-it-to-a-normal-item"></a>Pour vendre un article non stocké et le convertir en article normal
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Commandes vente**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau**. complétez les champs du raccourci **Général** comme pour toute commande vente.
3. Sur une nouvelle ligne vente, laissez le champ **Article** vide, sélectionnez **Ligne**, **Fonctions**, puis sélectionnez **Articles non stockés**.

    L'article non stocké est converti en un article normal. Une nouvelle fiche article pré-remplie avec les informations de l'article non stocké ainsi qu'un modèle d'article pertinent sont créés.
4. Dans la fenêtre **Articles non stockés**, sélectionnez l'article non stocké que vous souhaitez vendre, puis choisissez le bouton **OK**.
5. Lorsque les lignes commande vente sont renseignées, sélectionnez l'action **Valider**.

Vous pouvez ensuite remplir ou modifier les champs sur la nouvelle fiche article, le cas échéant. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md).

**Remarque** : un enregistrement de référence externe article est automatiquement créé pour le fournisseur de l'article entre le numéro article fournisseur et votre nouveau numéro article.

## <a name="see-also"></a>Voir aussi
[Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md)  
[Gestion du stock](inventory-manage-inventory.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

