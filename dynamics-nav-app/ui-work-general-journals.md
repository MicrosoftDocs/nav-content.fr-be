---
title: "Utilisation des feuilles comptabilité"
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
ms.openlocfilehash: 2dc2b22fbc0ff70addd16ca14e8c5416c49915e7
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="work-with-general-journals"></a>Utilisation des feuilles comptabilité
Les feuilles comptabilité vous permettent de valider des transactions financières dans les comptes généraux et dans d'autres comptes tels que les comptes bancaires, client et fournisseur. La validation avec une feuille comptabilité crée toujours des écritures dans les comptes généraux. C'est le cas même lorsque, par exemple, vous validez une ligne feuille dans un compte client, parce qu'une écriture est validée dans un compte client de la comptabilité via un groupe comptabilisation.

Les informations que vous saisissez dans une feuille sont temporaires et peuvent être modifiées tant qu'elles sont dans la feuille. Lorsque vous validez la feuille, les informations sont transférées vers des écritures de comptes individuels, où elles ne peuvent pas être modifiées. Toutefois, vous pouvez délettrer des écritures validées et valider des écritures de contrepassation ou de correction.

## <a name="journal-templates-and-batches"></a>Modèles feuilles et noms de feuilles
Il existe plusieurs modèles feuille. Chaque modèle feuille est représenté par une fenêtre dédiée avec des fonctions particulières et les champs nécessaires pour la prise en charge de ces fonctions, notamment la fenêtre **Feuille rapprochement bancaire** qui permet de traiter les paiements bancaires et la fenêtre **Feuille paiement** qui permet de payer vos fournisseurs.

Pour chaque modèle feuille, vous pouvez configurer votre propre feuille personnelle sous forme de nom de feuille. Par exemple, vous pouvez définir votre propre nom de feuille pour la feuille paiement dotée de votre présentation et de vos paramètres personnels.

**Remarque** : un exemple de paramètre personnel que vous pouvez définir dans votre nom feuille comptabilité consiste à faire en sorte que le système vous aide en remplissant automatiquement les champs. Si vous cochez la case **Suggérer le montant contrepartie** de la ligne pour votre nom feuille dans la fenêtre **Noms feuilles comptabilité**, le champ **Montant** dans, par exemple, les lignes feuille comptabilité pour le même numéro de document est automatiquement prérempli avec la valeur nécessaire à la contrepartie dans le document. Pour plus d'informations, reportez-vous à [Laisser Dynamics NAV suggérer des valeurs](ui-let-system-suggest-values.md).

## <a name="main-accounts-and-balancing-accounts"></a>Compte principaux et comptes contrepartie
Si vous avez configuré des comptes contrepartie par défaut pour les noms feuille, le compte contrepartie sera renseigné automatiquement lorsque vous renseignez le champ **N° compte**. . Sinon, remplissez les deux champs **N° compte** et **N° compte contrepartie** manuellement. Un montant positif dans le champ **Montant** est débité du compte principal et crédité dans le compte contrepartie. Un montant négatif est crédité sur le compte principal et débité du compte contrepartie.

**Remarque** : la TVA est calculée séparément pour le compte principal et le compte contrepartie, afin qu'ils puissent utiliser des taux de pourcentage de TVA différents.

## <a name="recurring-journals"></a>Feuilles abonnement
Une feuille récurrente est une feuille comptabilité contenant des champs spécifiques pour la gestion des transactions que vous validez fréquemment avec peu ou pas de modifications. Utilisez ces champs dans le cadre des transactions récurrentes pour valider les montants fixes et variables. Vous pouvez également définir des inversions automatiques d'écritures pour le lendemain de la date de validation et utiliser les clés de répartition avec les écritures récurrentes.

## <a name="see-also"></a>Voir aussi
[Procédure : utiliser les clés de ventilation dans les feuilles de comptabilité](ui-how-use-allocation-keys-general-journals.md)  
[Finance](finance-setup.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

