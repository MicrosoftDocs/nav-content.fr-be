---
title: "Créer et gérer des articles non stockés"
description: "Décrit comment commercialiser des articles non valorisable ou des articles qui ne sont pas mis à jour dans votre stock."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: non-inventoriable
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: dd1497d0727935d4954f826eceb303761850dada
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-nonstock-items"></a>Procédure : utiliser des articles non stockés
Vous pouvez proposer certains articles à vos clients pour leur rendre service, que vous ne souhaitez pas conserver en stock tant que vous ne commencez pas à les commercialiser. Lorsque vous souhaitez commencer à maintenir de tels articles en stock, vous pouvez les convertir en fiches article normales de deux façons.

* Depuis une fiche article non stocké, créez une nouvelle fiche article basée sur un modèle.
* Depuis une ligne commande vente de type **Article** avec un champ **N°* vide, sélectionnez un article non stocké. Une fiche article est automatiquement créée pour l'article non stocké.

> [!NOTE]  
>   Vous ne pouvez pas sélectionner d'article non stocké à partir de la fenêtre **Facture vente**. Vous pouvez sélectionner un article non stocké à partir de la fenêtre **Devis**, mais l'article non stocké ne sera pas converti en un article normal lorsque vous utilisez la fonction **Créer commande**.

Un article non stocké a généralement le numéro d'article du fournisseur qui le fournit. Pour activer la conversion d'une fiche article non stocké en une fiche article normale, vous devez tout d'abord configurer comment la numérotation de l'article fournisseur est convertie dans votre propre numérotation d'article.   

## <a name="to-create-a-nonstock-item"></a>Pour créer un article non stocké
Les fiches article non stocké ont moins d'informations que les fiches article normales, car vous ne les utilisez que pour proposer des devis ainsi que pour d'autres procédures. Pour cette raison, elles doivent être converties en fiches article normales, avant que vous puissiez valider les transactions commerciales pour elles.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Articles non stockés**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau**.
3. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-how-nonstock-item-numbers-are-converted-to-your-own-numbering"></a>Pour configurer comment les numéros d'article non stocké sont convertis en votre propre numérotation
Pour activer la conversion d'une fiche article non stocké en une fiche article normale, vous devez tout d'abord configurer comment la numérotation de l'article fournisseur est convertie dans votre propre format de numérotation d'article.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Paramètres art. non stockés**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins.

## <a name="to-convert-a-nonstock-item-to-a-normal-item"></a>Pour convertir un article non stocké en un article normal
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Articles non stockés**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche pour un article non stocké que vous pouvez convertir en un article normal.
3. Dans la fenêtre **Fiche article non stocké**, sélectionnez l'action **Créer un article**.

Une nouvelle fiche article pré-remplie avec les informations de l'article non stocké ainsi qu'un modèle d'article pertinent sont créés. Vous pouvez ensuite remplir ou modifier les champs sur la nouvelle fiche article, le cas échéant. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux articles](inventory-how-register-new-items.md).

## <a name="to-sell-a-nonstock-item-and-convert-it-to-a-normal-item"></a>Pour vendre un article non stocké et le convertir en article normal
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Commandes vente**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau**. Complétez les champs du raccourci **Général** comme pour toute commande vente. Pour en savoir plus, voir [Procédure : vendre des produits](sales-how-sell-products.md).
3. Sur une nouvelle ligne vente, dans le champ **Type**, sélectionnez **Article**, mais laissez le champ **N°** vide.
4. Choisissez l'action **Ligne**, puis l'action **Sélectionner articles non stockés**.

    L'article non stocké est converti en un article normal. Une nouvelle fiche article pré-remplie avec les informations de l'article non stocké ainsi qu'un modèle d'article pertinent sont créés.
5. Dans la fenêtre **Articles non stockés**, sélectionnez l'article non stocké que vous souhaitez vendre, puis choisissez le bouton **OK**.
6. Lorsque les lignes commande vente sont renseignées, sélectionnez l'action **Valider**.

Vous pouvez ensuite remplir ou modifier les champs sur la nouvelle fiche article, le cas échéant. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux articles](inventory-how-register-new-items.md).

> [!NOTE]  
>   Un enregistrement de référence externe article est automatiquement créé pour le fournisseur de l'article entre le numéro article fournisseur et votre nouveau numéro article.

## <a name="see-also"></a>Voir aussi
[Procédure : enregistrer de nouveaux articles](inventory-how-register-new-items.md)  
[Procédure : créer des commandes spéciales](sales-how-to-create-special-orders.md)|  
[STOCKS ET EN-COURS](inventory-manage-inventory.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

