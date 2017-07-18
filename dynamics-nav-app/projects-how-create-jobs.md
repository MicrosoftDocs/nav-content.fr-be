---
title: "Procédure : Créer des projets"
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: df34c435d07e9526cb4d93e2bfc30162258ba957
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-create-jobs"></a>Procédure : Créer des projets
Lorsque vous démarrez un nouveau projet, vous devez créer une fiche projet avec des tâches intégrées et des lignes planning structurées en deux couches.  

La première couche inclut les tâches du projet. Vous devez créer au moins une tâche par projet car toutes les validations font référence à une tâche de projet. Cela permet de configurer les lignes planning projet et de valider la consommation dans le projet.

La seconde couche inclut les lignes planning projet, qui spécifient l'utilisation détaillée des ressources, articles et diverses charges de comptabilité.

La structure de couche permet de séparer le projet en tâches plus petites et ainsi d'utiliser des détails plus spécifiques dans l'établissement du budget, les devis et l'enregistrement. En outre, elle vous donne un aperçu de la progression d'un projet. Par exemple, vous pouvez rechercher si vous respectez les étapes importantes fixées ou si vous êtes en passe de satisfaire les attentes budgétaires.

**Remarque** : L'action **Nouveau projet** du tableau de bord **Chef de projet** lance une configuration assistée qui vous guide dans les étapes de création d'un projet avec des tâches intégrées et des lignes planning. La procédure suivante décrit comment exécuter les étapes manuellement.

## <a name="to-create-a-job-card"></a>Pour créer une fiche projet
Vous devez créer une fiche projet, puis créez des Lignes tâche projet et des lignes planning projet pour ce projet.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projets**, puis sélectionnez le lien connexe.  
2. Cliquez sur **Nouveau**, puis renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Pour spécifier le projet avec les informations d'autres projets, cliquez sur **Copier projet**, renseignez les champs selon vos besoins, puis cliquez sur le bouton **OK**.

**REMARQUE** : Si vous utilisez des feuilles de temps dans le projet, vous devez également indiquer une personne responsable. Cette personne peut approuver les feuilles de temps pour les tâches des salariés associées à ce projet. Pour plus d'informations, reportez-vous à [Procédure : Paramétrer des feuilles de temps](projects-how-setup-time-sheets.md).

## <a name="to-create-tasks-for-a-job"></a>Pour créer une tâche pour un projet  
L'une des clés de la création d'un projet consiste à spécifier les différentes tâches impliquées dans le projet. Pour ce faire, ajoutez de nouvelles lignes dans le raccourci **Tâches** de la fenêtre **Fiche projet**, une tâche par ligne. Chaque projet doit avoir au minimum une tâche.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projets**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche projet pour un projet concerné.
3. Sur le raccourci **Tâches**, renseignez les champs, le cas échéant sur une ligne.
4. Pour indenter des tâches et créer une hiérarchie, cliquez sur **Tâches**, puis sur **Indenter tâches projet**.
5. Répétez les étapes 3 et 4 pour toutes les tâches dont vous avez besoin pour le projet.
6. Pour spécifier les tâches du projet avec les informations d'autres tâches de projet, cliquez sur **Copier les tâches projet de**, renseignez les champs selon vos besoins, puis cliquez sur le bouton **OK**.

## <a name="to-create-planning-lines-for-a-job"></a>Pour créer des lignes planning pour un projet  
Vous pouvez redéfinir vos nouvelles tâches projet sur les lignes planning projet. Une ligne planning peut être utilisée pour extraire toute information que vous souhaitez suivre pour un projet. Vous pouvez utiliser des lignes planning pour ajouter des informations telles que les ressources nécessaires ou pour capturer les articles nécessaires pour exécuter le projet. Par exemple, si vous avez une tâche pour obtenir l'accord d'un client sur un projet, vous pouvez associer cette tâche à des lignes planning article, comme un rendez-vous avec le client ou l'affectation d'une ressource.  

Une ligne planning projet peut avoir l'un des types suivants :  

|Type|Désignation|
|----|-----------|
|**Budget**|Permet d'obtenir les activités et coûts prévus pour le projet, généralement dans le cadre d'un projet de régie. Les lignes planning de ce type ne peuvent pas être facturées.|
|**Facturable**|Permet de fournir un devis au client, généralement utilisé dans le cadre d'un projet à prix fixe.|
|**Budget et Facturable**|Permet de faire correspondre l'activité budgétée au montant que vous souhaitez facturer.|  

**Remarque**. Au fur et à mesure de l'ajout d'informations sur les lignes planning projet, le coût est automatiquement mis à jour. Par exemple, le coût, le prix et la remise relatifs aux ressources et aux articles sont initialement calculés sur la base des informations définies dans les fiches ressource et article.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projets**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche projet appropriée.
3. Sélectionnez une tâche projet pour laquelle le champ **Type tâche projet** contient **Validation** puis, cliquez sur **Lignes planning projet**.  
4. Dans la fenêtre **Lignes planning projet**, renseignez les champs, le cas échéant sur une nouvelle ligne.
5. Répétez les étapes 3 et 4 pour toutes les lignes planning dont vous avez besoin pour la tâche projet.

## <a name="see-also"></a>Voir aussi
[Gérer des projets](projects-manage-projects.md)  
[Finance](finance-setup.md)  
[Gestion des achats](purchasing-manage-purchasing.md)         
[Gestion des ventes](sales-manage-sales.md)      
[Utiliser Dynamics NAV](ui-work-product.md)  

