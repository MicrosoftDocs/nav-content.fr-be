---
title: Configuration des axes analytiques
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1b7a293982dfc7ff73c163ad1711e2bce098e98e
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---

# <a name="set-up-dimensions"></a>Configuration des axes analytiques
Vous devez définir les axes et les sections analytiques que vous souhaitez utiliser dans votre société. Vous devez également définir les axes analytiques que vous souhaitez utiliser comme axes principaux et comme raccourcis axe. Prenez soin de définir en tant qu'axes principaux et raccourcis axe pour votre société les axes analytiques les plus efficaces.  
Paramétrez tous les différents axes dont vous souhaitez effectuer le suivi dans la fenêtre **Axes analytiques**. La fenêtre Axes analytiques contient une ligne pour chaque axe, tel que *Projet*, *Département*, *Zone* et *Commercial*.  

Pour chaque axe analytique, vous devez également configurer les sections analytiques, par exemple, tous les départements de votre société. Les sections analytiques peuvent être paramétrées sous forme de structure hiérarchique similaire au plan comptable, de manière à ce que les données puissent être réparties en plusieurs niveaux de granularité et à ce que des sous-ensembles de sections analytiques puissent être totalisés.  

Vous pouvez définir deux axes principaux qui seront automatiquement disponibles partout, par exemple dans les états et les traitements par lots. Vous pouvez également définir six raccourcis axe supplémentaires qui seront disponibles sous forme de champ dans les lignes feuille et document. Pour utiliser les axes restants, vous pouvez y accéder via une fenêtre séparée qui affiche les axes pour la ligne.  

Vous pouvez définir autant d'axes et de sections analytiques pour chaque axe que nécessaire pour votre société. Vous pouvez utiliser tous les axes analytiques que vous avez définis dans les écritures des feuilles et des documents, ainsi que dans les états et les traitements par lots liés aux axes analytiques.  

## <a name="set-up-default-dimensions-for-customers-vendors-and-other-accounts"></a>Configuration des axes analytiques par défaut pour les clients, les fournisseurs, et les autres comptes
Vous pouvez configurer une affectation analytique pour un compte spécifique. Ce code est ensuite copié dans la feuille ou le document lorsque le champ du numéro du compte est renseigné sur la ligne. Toutefois, vous pouvez supprimer ou modifier le code si nécessaire. Vous pouvez également rendre un axe analytique obligatoire afin qu'il soit impossible de valider une écriture avec un type de compte spécifique sauf si une section analytique lui est affectée.  

En outre, vous pouvez configurer un axe analytique par défaut pour chaque type de compte de sorte que ce code soit copié vers la feuille ou le document lorsque le type de compte est renseigné sur la ligne. Cependant, vous pouvez toujours modifier le code dans le document si nécessaire.  

Enfin, vous pouvez également rendre un axe analytique obligatoire afin qu'il soit impossible de valider une écriture avec un type de compte spécifique sauf si une section analytique lui est affectée.

## <a name="see-also"></a>Voir aussi
[Utilisation des axes analytiques](finance-dimensions.md)  
[Configurer les processus financiers de base](finance-setup-finance.md)

