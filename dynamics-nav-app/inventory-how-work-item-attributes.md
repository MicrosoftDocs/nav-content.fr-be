---
title: "Procédure : utilisation des attributs d'article"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: eaf539f1d4d00c2cd5679f39f29a3428e33ee1fd
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-item-attributes"></a>Procédure : utilisation des attributs d'article
Lorsque les clients recherchent des renseignements au sujet d'un article, par courrier ou via une boutique en ligne, ils peuvent effectuer leur recherche en fonction de caractéristiques, telles que la hauteur et l'année du modèle. Pour assurer le service de ce client, vous pouvez affecter des valeurs attribut article de différents types à vos articles, qui peuvent être utilisées pour rechercher les articles.

Vous pouvez également allouer les attributs d'article aux catégories d'article, qui s'appliquent ensuite aux articles qui utilisent les catégories d'article. Pour plus d'informations, voir [Procédure : catégoriser des articles](inventory-how-categorize-items.md).

## <a name="to-create-item-attributes"></a>Pour créer des attributs d'article
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Attributs d'article**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Attributs d'article**, sélectionnez l'action **Nouveau**.
3. Dans la fenêtre **Attribut article**, renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

**Remarque** : si vous sélectionnez **Option** dans le champ **Type**, vous pouvez sélectionner l'action **Valeurs attribut article** afin de créer des valeurs pour l'attribut d'article. Pour en savoir plus, voir la section « Pour créer des valeurs pour les attributs d'article de type Option ».  

## <a name="to-create-values-for-item-attributes-of-type-option"></a>Pour créer des valeurs pour les attributs d'article de type Option
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Attributs d'article**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Attributs article**, sélectionnez un attribut d'article de type Option pour lequel vous souhaitez créer des valeurs, puis sélectionnez l'action **Valeurs attribut article**.
3. Dans la fenêtre **Valeurs attribut article**, renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

## <a name="to-assign-item-attributes-to-items"></a>Pour allouer des attributs article à des articles
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Articles**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Articles**, sélectionnez l'article auquel vous souhaitez affecter des attributs article, puis sélectionnez l'action **Attributs**.
3. Dans la fenêtre **Valeurs d'attribut d'article**, sélectionnez l'action **Nouveau**.
4. Sélectionnez le bouton AssistEdit dans le champ **Attribut** et sélectionnez un attribut d'article existant. Sinon, sélectionnez l'action **Nouveau** pour créer tout d'abord un nouvel attribut comme expliqué dans la section « Créer des attributs d'article ».
5. Dans le champ **Valeur**, saisissez la valeur d'attribut article, telle que « 2010 » pour l'attribut de l'année modèle.
6. Pour les attributs d'article de type Option, sélectionnez le bouton AssistEdit dans le champ **Valeur** et sélectionnez une valeur d'attribut d'article. Sinon, sélectionnez l'action **Nouveau** pour créer tout d'abord une nouvelle valeur d'attribut comme expliqué dans la section « Créer des valeurs pour les attributs d'article de type Option ».
7. Répétez les étapes 4 à 6 pour tous attributs article que vous souhaitez affecter à l'article.

## <a name="to-assign-item-attributes-to-item-categories"></a>Pour allouer des attributs article aux catégories article
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Catégories d'article**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Catégories d'article**, sélectionnez la catégorie article à laquelle vous souhaitez affecter des attributs article, puis sélectionnez l'action **Modifier**.
3. Dans la fenêtre **Fiche catégorie article**, sur le raccourci **Attributs**, sélectionnez l'action **Nouveau**.
4. Sélectionnez le bouton AssistEdit dans le champ **Attribut** et sélectionnez un attribut d'article existant. Sinon, sélectionnez l'action **Nouveau** pour créer tout d'abord un nouvel attribut comme expliqué dans la section « Créer un attribut article ».
5. Dans le champ **Valeur par défaut**, cliquez sur le bouton AssistEdit et sélectionnez une valeur attribut article.
6. Répétez les étapes 4 et 5 pour tous attributs article que vous souhaitez affecter à la catégorie d'article.

**Remarque** : les attributs article pour les catégories d'article seront transmis aux catégories d'article enfant. Cela est indiqué par le champ **Hérité de** sur le raccourci **Attributs**. Pour plus d'informations, voir [Procédure : catégoriser des articles](inventory-how-categorize-items.md).

## <a name="to-filter-by-item-attributes"></a>Pour filtrer par attribut d'article
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Articles**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Articles**, sélectionnez l'action **Filtrer par attributs**.
3. Dans la fenêtre **Filtrer les articles par attribut**, cliquez sur le bouton AssistEdit du champ **Attribut**, puis sélectionnez un attribut article.
4. Dans le champ **Valeur**, cliquez sur le bouton AssistEdit et sélectionnez une valeur attribut selon laquelle filtrer les articles.

    **Remarque** : vous pouvez uniquement sélectionner des valeurs directement pour les attributs article dotés de valeurs fixes, telles que Couleur. Pour modifier des attributs article dotés de valeurs variables, telles que Largeur, vous devez spécifier la valeur attribut article en sélectionnant d'abord une condition. Reportez-vous à l'étape 5.
5. Dans le champ **Valeur** d'un attribut article variable, cliquez sur le bouton AssistEdit.
6. Dans la fenêtre **Spécifier la valeur du filtre**, dans le champ **Condition**, cliquez sur la flèche déroulante et sélectionnez une condition.
7. Dans le champ **Valeur**, saisissez une valeur attribut selon laquelle filtrer les articles.

    **Exemple** : pour filtrer les articles pour lesquels la description matière se termine par « bleu », renseignez les champs comme suit : champ **Attribut** : Description matière, champ **Condition** : Se termine par, champ **Valeur** : bleu.
8. Cliquez sur le bouton **OK**.   

Les articles de la fenêtre **Articles** sont filtrés selon les valeurs attribut article spécifiées.

## <a name="see-also"></a>Voir aussi
[Procédure : catégoriser des articles](inventory-how-categorize-items.md)    
[Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md)  
[Gestion du stock](inventory-manage-inventory.md)  
[Utiliser Dynamics NAV](ui-work-product.md)
