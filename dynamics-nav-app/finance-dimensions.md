---
title: Axes analytiques
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a1b38e74717e87bea6efb46f8f4e5236b6ec4e64
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

#<a name="dimensions"></a>Axes analytiques
Les axes sont des données que vous ajoutez aux écritures pour les catégoriser à des fins d'analyse. Par exemple, certains axes peuvent indiquer de quel projet ou département provient une écriture.
Vous pouvez alors utiliser les axes analytiques au lieu de configurer des comptes généraux distincts pour chaque département et projet. Cela vous permet d'avoir des informations d'analyse riches dans vos données sans avoir besoin d'utiliser un plan comptable complexe.
Vous pouvez définir un nombre d'axes illimité avec un nombre de sections analytiques illimité.  

Par exemple, vous configurez un axe analytique appelé *Département*, et vous utilisez cet axe et une section analytique lorsque vous validez des documents vente. Ensuite, vous pouvez ultérieurement obtenir les données de veille économique, par exemple sur quels articles ont été vendus par quels départements.
Plus vous configurez et utilisez d'axes analytiques, plus vous pouvez baser vos décisions commerciales sur des états détaillés. Par exemple, une seule écriture vente peut comporter plusieurs informations analytiques : le compte sur lequel la vente de l'article a été validée, l'endroit où l'article a été vendu, le nom du vendeur et le type de client qui a effectué l'achat.  

## <a name="using-dimensions"></a>Utilisation des axes analytiques
Dans un document tel qu'une commande vente, vous pouvez ajouter des informations analytiques pour une seule ligne document et pour le document lui-même. Par exemple, dans la fenêtre **Commande vente**, vous pouvez saisir des sections analytiques pour les deux premiers raccourcis axe directement dans le document et ajouter des informations analytiques complémentaires si vous cliquez sur le bouton **Axes analytiques**.  
Si vous travaillez plutôt sur une feuille, vous pouvez également ajouter à une écriture des informations analytiques de la même manière, si vous avez configuré des raccourcis axe en tant que champs directement dans les lignes feuille.  
Vous pouvez configurer des axes analytiques par défaut pour des comptes ou des types de compte, de sorte que les axes et les sections analytiques soient renseignés automatiquement.  

## <a name="dimension-sets"></a>Ensembles de dimensions
Un ensemble de dimensions est une combinaison unique de sections analytiques. Il est stocké comme des écritures de l'ensemble de dimensions dans la base de données. Chaque écriture de l'ensemble de dimensions représente une section analytique unique. L'ensemble de dimensions est identifié par un ID courant, qui est affecté à chaque écriture correspondante qui appartient à l'ensemble de dimensions.  

Lorsque vous créez une ligne de feuille, un en-tête de document ou une ligne de document, vous pouvez spécifier une combinaison de sections analytiques. Au lieu d'enregistrer explicitement chaque section analytique dans la base de données, un ID d'ensemble de dimensions est affecté à la ligne de feuille, à l'en-tête du document ou à la ligne du document pour spécifier l'ensemble de dimensions.  

## <a name="see-also"></a>Voir aussi
[Finance](finance-setup.md)  
[Configuration des axes analytiques](finance-setup-setup-dimensions.md)  

