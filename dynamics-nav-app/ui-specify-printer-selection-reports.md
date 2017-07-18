---
title: "Spécifier la sélection de l'imprimante pour les états"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 55b48aef2bc108ced7f581f0ff6c11263ee467df
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---
    
# <a name="specify-printer-selection-for-reports"></a>Spécifier la sélection de l'imprimante pour les états
Vous pouvez configurer les états de sorte qu'ils soient imprimés sur une imprimante spécifique. Voici quelques exemples de sélections d'imprimante : 

- Vous pouvez imprimer des états sur un en-tête de la société.
- Vous pouvez imprimer des états sur des formats de papier différents.
- Vous pouvez imprimer des états sur l'imprimante par défaut d'un employé spécifié.

La fenêtre **Sélections d'imprimantes** pour définir différentes valeurs afin d'obtenir des sorties différentes. Si vous configurez une sélection d'imprimante spécifique, cette sélection a priorité sur une sélection d'imprimante plus générale. Par exemple, vous pouvez configurer une sélection d'imprimante en entrant une valeur dans les champs **ID utilisateur**, **ID état** et **Nom de l'imprimante**. Cette sélection d'imprimante a priorité sur une sélection d'imprimante dont les champs **ID utilisateur** ou **ID état** sont vides. 

Le tableau suivant décrit les combinaisons de valeurs à spécifier lors de la configuration de sélections d'imprimante pour un état.

|Pour                                                 |Configurez les valeurs suivantes                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|Imprimer un état sur une imprimante spécifique pour tous les utilisateurs |Spécifiez une valeur dans les champs **ID état** et **Nom de l'imprimante** et ne renseignez pas le champ **ID utilisateur**.|
|Imprimer tous les états sur une imprimante spécifique pour un utilisateur spécifique|Spécifiez une valeur dans les champs **ID utilisateur** et **Nom de l'imprimante** et ne renseignez pas le champ **ID état**.|
|Définir l'imprimante par défaut pour tous les états|Spécifiez une valeur dans le champ **Nom de l'imprimante** et ne renseignez pas les champs **ID utilisateur** et **ID état**.|
|Imprimer un état spécifique sur l'imprimante par défaut de l'utilisateur|Spécifiez une valeur dans le champ **ID état** et ne renseignez pas les champs **Nom de l'imprimante** et **ID utilisateur**.|
|Imprimer un état spécifique sur une imprimante spécifique pour un utilisateur spécifique|Spécifiez une valeur dans les trois champs.|

## <a name="see-also"></a>Voir aussi
[Utiliser Dynamics NAV](ui-work-product.md)

