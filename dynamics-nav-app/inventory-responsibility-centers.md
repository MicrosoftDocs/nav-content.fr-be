---
title: "Procédure : utiliser les centres de gestion"
description: "Les centres de gestion permettent de gérer les centres administratifs. Un centre de gestion peut être un centre de coûts, un centre de profit, un centre d'investissement ou tout autre centre administratif défini par la société."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d857daec1c6ab73639783e03e6592c0958fe2f70
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-responsibility-centers"></a>Procédure : utiliser les centres de gestion
Les centres de gestion permettent de gérer les centres administratifs. Un centre de gestion peut être un centre de coûts, un centre de profit, un centre d'investissement ou tout autre centre administratif défini par la société. Un bureau de vente, un département d'achat pour plusieurs emplacements, un bureau de planification d'usine, etc. sont des exemples de centres de gestion. Par exemple, cette fonctionnalité permet aux sociétés de paramétrer des vues spécifiques à l'utilisateur des documents vente et achat associés exclusivement à un centre de gestion particulier.  

L'utilisation de plusieurs magasins avec des centres de gestion permet de gérer les activités commerciales de façon flexible et optimale.

Des magasins multiples permettent aux sociétés de gérer leur stock dans plusieurs magasins au moyen d'une seule base de données. Deux concepts, des magasins et des points de stock, sont les pierres angulaires du granule. Un magasin est défini comme un lieu qui gère l'emplacement physique et la quantité des articles. Le concept est assez étendu pour inclure des magasins tels que les usines ou les unités de fabrication et les centres de distribution, les entrepôts, les magasins d'exposition et les véhicules de service. Un point de stock est défini comme un article d'un magasin spécifique et/ou comme une variante. Grâce aux points de stock, les sociétés utilisant plusieurs magasins peuvent ajouter des informations de réapprovisionnement, des adresses et des informations financières de validation au niveau du magasin. Elles peuvent ainsi réapprovisionner les variantes du même article dans chaque magasin et commander des articles pour chaque magasin d'après les informations de réapprovisionnement spécifiques du magasin.  

Les centres de gestion élargissent la fonction de magasins multiples en permettant aux utilisateurs de gérer les centres administratifs. Un centre de gestion peut être un centre de coûts, une centre de profit, un centre d'investissement ou tout autre centre administratif défini par la société. Un bureau de vente, un département d'achat pour plusieurs emplacements, un bureau de planification d'usine, etc. sont des exemples de centres de gestion. Par exemple, cette fonctionnalité permet aux sociétés de paramétrer des vues spécifiques à l'utilisateur des documents vente et achat associés exclusivement à un centre de gestion particulier.

## <a name="to-set-up-a-responsibility-center"></a>Pour configurer un centre de gestion  
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Centres de gestion**, puis sélectionnez le lien connexe.  
2.  Sélectionnez l'action **Nouveau**.  
3.  Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    Si vous utilisez des centres de gestion pour administrer votre société, il peut être utile de définir un centre de gestion par défaut pour votre société.
4. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Informations société**, puis sélectionnez le lien connexe.
5. Dans le champ **Centre de gestion**, entrez un code centre de gestion.

Ce code est utilisé sur tous les documents achat, vente ou service si l'utilisateur, le client ou le fournisseur n'a pas de centre de gestion par défaut. Sur un document vente, achat ou service, vous pouvez saisir un autre centre de gestion à la place de la valeur par défaut.

> [!NOTE]  
>  Lorsque vous saisissez un code centre de gestion sur un document, le programme affecte l'adresse, les axes et les prix indiqués sur le document.  

## <a name="to-assign-responsibility-centers-to-users"></a>Pour affecter des centres de gestion à des utilisateurs  
Vous pouvez configurer des utilisateurs de sorte que, dans leurs routines quotidiennes, le programme récupère uniquement les documents propres à leur activité. Les utilisateurs sont généralement associés à un centre de gestion et utilisent uniquement les documents propres à des modules spécifiques de ce centre.  

Pour configurer cela, vous devez affecter des centres de gestion à des utilisateurs dans trois modules : Achats, Ventes et Gestion des services.  

1.  Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Paramètres utilisateur**, puis choisissez le lien associé.  
2.  Dans la fenêtre **User Setup**, sélectionnez l'utilisateur auquel vous souhaitez affecter un centre de gestion. Si l'utilisateur ne figure pas dans la liste, saisissez un code utilisateur dans le champ **Code utilisateur**.  
3.  Dans le champ **Filtre centre gestion vente**, indiquez le centre de gestion dans lequel l'utilisateur aura des tâches liées aux ventes.  
4.  Dans le champ **Filtre centre gestion achat**, indiquez le centre de gestion dans lequel l'utilisateur aura des tâches liées aux achats.  
5.  Dans le champ **Filtre centre gestion service**, indiquez le centre de gestion dans lequel l'utilisateur aura des tâches liées à la gestion des services.  

> [!NOTE]  
>  Les utilisateurs peuvent visualiser toutes les écritures comptables et tous les documents validés ; ils ne sont pas limités à ceux de leur centre de gestion.

## <a name="see-also"></a>Voir aussi  
[Configuration de stock](inventory-setup-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)
[Stock](inventory-manage-inventory.md)[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[Gestion d'entrepôt](warehouse-manage-warehouse.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

