---
title: "Configurer des relations d'affaires sur des sociétés contact"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 20abe2f08fc726a008719f94389579d02ecbd275
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---
# <a name="set-up-business-relations-on-contact-companies"></a>Configurer des relations d'affaires sur des sociétés contact
Les relations d'affaires vous permettent d'indiquer les rapports établis avec vos contacts, tels que les prospects, les banques, les consultants, les prestataires de services, et ainsi de suite.

L'utilisation des relations d'affaires sur les contacts processus en deux étapes. Tout d'abord, vous définissez le code relation d'affaires. Vous ne devez effectuer cette étape qu'une seule fois pour chaque relation d'affaires. Une fois que vous disposez d'un code relation d'affaires, vous pouvez commencer à affecter le code aux sociétés contact.

**Remarque** : si vous prévoyez de synchroniser vos contacts avec des fournisseurs, des clients ou des comptes bancaires dans d'autres parties de l'application, vous pouvez configurer pour eux une relation d'affaires.

## <a name="define-a-business-relation-code"></a>Définir un code relation d'affaires
Le code relation d'affaires définit une catégorie ou un type de relation d'affaires, telles que BANQUE ou AVOCAT. Vous pouvez disposer de plusieurs codes relation d'affaires. Pour définir la relation d'affaires, vous utilisez la fenêtre **Relations d'affaires**.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Relations d'affaires**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau**, et entrez un code et une désignation. Vous pouvez saisir pour le code un maximum de 11 caractères, et toute combinaison de chiffres et des lettres.

## <a name="assign-business-relations-to-a-contact"></a>Affecter des relations d'affaires à un contact
Vous ne pouvez pas affecter de relations d'affaires à un individu, mais uniquement à des sociétés.

1. Ouvrez le contact.
2. Sélectionnez l'action **Société**, puis l'action **Relations d'affaires**.

    La fenêtre **Relations d'affaires contact** s'ouvre.
3. Dans le champ **Code relation d'affaires**, sélectionnez la relation d'affaires à affecter.

Répétez ces étapes pour chaque relation d'affaires à affecter. Vous pouvez également affecter des relations d'affaires à partir de la liste des contacts en suivant la même procédure.

Le nombre de relations d'affaires que vous avez affectées au contact s'affiche dans le champ **Nbre relations d'affaires** de la section **Segmentation** de la fenêtre **Contact**.

Une fois que vous avez affecté des relations d'affaires à vos contacts, vous pouvez utiliser ces informations pour sélectionner des contacts pour vos segments. Pour plus d'informations, reportez-vous à [Procédure : ajouter des contacts à des segments](marketing-add-contact-segment.md).

##<a name="see-also"></a>Voir aussi
[Création de sociétés contact](marketing-create-contact-companies.md)

