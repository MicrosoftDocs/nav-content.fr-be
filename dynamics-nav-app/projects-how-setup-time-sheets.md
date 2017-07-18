---
title: "Procédure : Paramétrer des feuilles de temps"
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
ms.openlocfilehash: 6cbacce79ce185d6ed00ea8383259d1b28f9e11b
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-time-sheets"></a>Procédure : paramétrer des feuilles de temps
Dans Dynamics NAV, les feuilles de temps gèrent l'enregistrement des heures sur une base hebdomadaire par incrément de sept jours. Elles permettent de suivre le temps consacré à des projets, et vous pouvez les utiliser pour enregistrer les heures ressource. Avant de pouvoir utiliser des feuilles de temps, vous devez les configurer.

Une fois l'utilisation des feuilles de temps au sein de votre organisation configurée, vous pouvez indiquer si et comment les feuilles de temps sont approuvées. Selon les besoins de votre organisation, vous pouvez désigner :

- un ou plusieurs utilisateurs en tant qu'administrateur et approbateur de feuille de temps pour toutes les feuilles de temps ;
- un approbateur de feuille de temps pour chaque ressource.

Lorsque vous créez des feuilles de temps, vous pouvez créer des feuilles de temps pour les ressources, les affecter aux lignes planning projet, et valider les lignes de feuille de temps. Pour plus d'informations, reportez-vous à [Procédure : Utiliser des feuilles de temps](projects-how-use-time-sheets.md).

## <a name="to-set-up-general-information-for-time-sheets"></a>Pour configurer des informations générales pour les feuilles de temps  

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres ressources**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Sélectionnez l'une des options suivantes pour le champ **Feuille de temps par approbation de projet**.

|Option |Désignation|
|---|---|
|**Jamais**|L'utilisateur du champ **ID utilisateur de l'approbateur de la feuille de temps** de la fiche ressource approuve la feuille de temps.|
|**Toujours**|L'utilisateur du champ **Responsable** de la fiche projet approuve la feuille de temps.|
|**Poste uniquement**|Si la feuille de temps poste est liée à un projet, alors l'utilisateur du champ **Responsable** spécifié sur la fiche projet approuve la feuille de temps. Si la feuille de temps poste est liée à une ressource, alors l'utilisateur du champ **ID utilisateur de l'approbateur de la feuille de temps** spécifié sur la fiche ressource approuve la feuille de temps.

## <a name="to-assign-a-time-sheet-administrator"></a>Pour affecter un administrateur de feuille de temps  

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres utilisateur**, puis sélectionnez le lien connexe.  
2.  Ajoutez un nouvel utilisateur (si la personne que vous souhaitez désigner en tant qu'administrateur de feuille de temps ne figure pas dans la liste des utilisateurs). Pour plus d'informations, contactez votre administrateur.  
3. Sélectionnez l'utilisateur qui deviendra l'administrateur de feuille de temps et sélectionnez la case à cocher **Admin. feuille de temps** .  

**Astuce** : Il est recommandé de ne désigner qu'un seul utilisateur en tant qu'administrateur de feuille de temps dans une société. Dans la procédure suivante, vous devez configurer un propriétaire et un approbateur de feuille de temps et affecter l'approbateur à chaque ressource.  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a>Pour affecter un propriétaire et un approbateur de feuille de temps  

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Ressources**, puis sélectionnez le lien connexe.
2. Sélectionnez la ressource pour laquelle vous souhaitez configurer la capacité d'utiliser des feuilles de temps, puis sélectionnez la case à cocher **Utiliser la feuille de temps**.  
3. Entrez l'ID du propriétaire de la feuille de temps dans le champ **ID utilisateur du propriétaire de la feuille de temps**. Le propriétaire peut entrer le temps d'utilisation dans une feuille de temps et la soumettre pour approbation. En règle générale, lorsque la ressource est une personne, cette personne est également le propriétaire.  
4. Entrez l'ID de l'approbateur de la feuille de temps dans le champ **ID utilisateur de l'approbateur de la feuille de temps**. L'approbateur peut approuver, rejeter ou rouvrir une feuille de temps.  

**Remarque** : Vous ne pouvez pas modifier l'ID de l'approbateur de feuille de temps s'il existe des feuilles de temps qui n'ont pas encore été traitées et dont le statut est **Soumis** ou **En cours**.

## <a name="see-also"></a>Voir aussi
[Configurer la gestion de projet](projects-setup-projects.md)  
[Gérer des projets](projects-manage-projects.md)  
[Finance](finance-setup.md)  
[Gestion des achats](purchasing-manage-purchasing.md)         
[Gestion des ventes](sales-manage-sales.md)      
[Utiliser Dynamics NAV](ui-work-product.md)  

