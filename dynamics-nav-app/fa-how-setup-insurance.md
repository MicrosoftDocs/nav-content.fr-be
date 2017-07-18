---
title: "Procédure : configurer une assurance immobilisation"
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
ms.openlocfilehash: 44bb5f20702a01d9fbbc025889ec2bc3191813be
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-insurance"></a>Procédure : configurer une assurance immobilisation
Pour gérer la couverture d'assurance des immobilisations, vous devez tout d'abord configurer certaines informations générales d'assurance ainsi qu'une fiche assurance par police.

## <a name="to-set-up-general-insurance-information"></a>Pour définir des informations générales relatives aux assurances  
Pour utiliser les fonctions d'assurance dans Dynamics NAV, vous devez définir certaines informations générales relatives aux assurances.  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Paramètres immobilisations**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.  

## <a name="to-set-up-insurance-types"></a>Pour définir des types d'assurance  
Vous pouvez regrouper vos polices d'assurance en catégories (assurances contre le vol, assurances incendie, etc.). Les types d'assurance sont utilisés sur la fiche assurance.
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Types d'assurance**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins.

## <a name="to-set-up-insurance-cards"></a>Pour définir des fiches assurance  
Vous pouvez rassembler des informations sur chaque police d'assurance dans la fiche assurance.  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Assurance**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Assurance**, sélectionnez l'action **Nouveau** pour créer une fiche assurance.  
3. Renseignez les champs selon vos besoins.

## <a name="to-set-up-insurance-journal-templates"></a>Pour définir des modèles feuille assurance  
Dynamics NAV crée automatiquement un modèle feuille assurance la première fois que vous ouvrez la fenêtre **Feuille assurance**. Vous pouvez cependant définir d'autres modèles feuille. Pour plus d'informations, reportez-vous à [Utilisation des feuilles comptabilité](ui-work-general-journals.md).  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Modèles feuille assurance**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins.

## <a name="to-set-up-insurance-journal-batches"></a>Pour définir des noms de feuille assurance  
Vous pouvez définir des feuilles dans un modèle feuille assurance. Les valeurs de la feuille servent de valeurs par défaut si les champs ne sont pas renseignés dans les lignes feuille. Pour en savoir plus, voir [Utiliser des feuilles comptabilité](ui-work-general-journals.md)  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Modèles feuille assurance**, puis sélectionnez le lien connexe.  
2. Sélectionnez un modèle feuille assurance, puis l'action **Lots**.
3. Dans la fenêtre **Lots feuille assurance**, renseignez les champs selon vos besoins.

**REMARQUE** : les numéros remplissent une fonction spéciale dans les noms de feuille. Si un nom de feuille ou de modèle feuille indique un numéro, ce numéro est incrémenté automatiquement de 1 à chaque fois que la feuille est validée. Par exemple, si vous saisissez HH1 dans le champ **Nom**, la feuille prend le nom HH2 après validation de la feuille HH1.

## <a name="see-also"></a>Voir aussi
[Configurer des immobilisations](fa-setup.md)  
[Gérer des immobilisations](fa-manage.md)  
[Finance](finance-setup.md)  
[Bienvenue dans Dynamics NAV](across-get-started.md)

