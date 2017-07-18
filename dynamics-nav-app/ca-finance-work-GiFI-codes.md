---
title: "Procédure : utilisation des codes IGRF au Canada"
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 695bca0a6836c47610210b759ae48af27484761f
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-work-with-gifi-codes-in-canada"></a>Procédure : utilisation des codes IGRF au Canada
Les informations fiscales peuvent inclure des comptes généraux, des états, des comptes de gestion, des bilans et des relevés des bénéfices non répartis. Les informations fiscales sont classifiées par le biais de codes. L'utilisation de codes aide le gouvernemental à traiter les informations, à préparer l'archivage électronique et à valider les informations fiscales par voie électronique. L'utilisation de codes aide également les organisations statistiques à travailler plus efficacement, en rendant les données financières plus facilement disponibles. Pour plus d'informations, reportez-vous au [site Web de l'Agence de revenu du Canada](http://www.cra-arc.gc.ca/).

L'Agence de revenu du Canada utilise les codes IGRF (Index général des renseignements financiers) pour recueillir, valider et traiter les informations financières et fiscales par voie électronique. Les meilleures pratiques suggèrent d'attribuer des codes IGRF uniquement aux comptes de validation, afin que tous les totaux soient calculés par votre logiciel d'établissement des déclarations fiscales.

Lorsqu'un compte est associé à un code IGRF, il est enregistré auprès de l'Agence de revenus sous ce code. Plusieurs comptes peuvent avoir le même code IGRF, mais chaque compte doit avoir un seul code IGRF.

Vous pouvez exporter les informations de solde par code IGRF et enregistrer le fichier exporté dans Excel, ce qui est utile pour transférer des informations vers votre logiciel d'établissement des déclarations fiscales.

## <a name="to-set-up-gifi-codes"></a>Pour configurer des codes IGRF
Dans Dynamics NAV, vous devez configurer des codes IGRF pour les comptes généraux, les états, les comptes de gestion, les comptes de résultat et les relevés de bénéfices non répartis.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Codes IGRF**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Codes IGRF**, sélectionnez l'action **Nouveau**.
3. Configurer les codes IGRF en renseignant les champs. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

## <a name="to-associate-gifi-codes-with-gl-accounts"></a>Pour associer des codes IGRF avec des comptes généraux
Pour enregistrer des données financières par code IGRF, chaque code IGRF doit être associé aux comptes appropriés dans le plan comptable.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Plan comptable**, puis sélectionnez le lien connexe.
2. Sélectionnez un compte général approprié, puis sélectionnez l'action **Modifier**.
3. Sur le raccourci **Comptabilité analytique**, dans le champ **Code IGRF**, sélectionnez un code IGRF approprié.

## <a name="to-view-account-balances-using-the-gifi-code-report"></a>Pour afficher les soldes de compte à l'aide de l'état de code IGRF
Vous pouvez consulter vos soldes de compte par code IGRF par le biais de l'état **Soldes de compte par code IGRF**.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Soldes de compte par code IGRF**, puis sélectionnez le lien connexe.
2. Spécifiez les éléments à inclure dans l'état en renseignant les champs. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Cliquez sur le bouton **Imprimer** ou **Aperçu**.

## <a name="to-export-balance-information-using-gifi-codes"></a>Pour exporter les informations de solde à l'aide de codes IGRF
Vous pouvez exporter les informations de solde à l'aide de codes IGRF et enregistrer le fichier exporté dans Excel. Vous pouvez modifier, enregistrer ou supprimer, le fichier. Ce fichier vous permet de transférer des informations vers votre logiciel d'établissement des déclarations fiscales.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Exporter les info IGRF dans Excel**, puis sélectionnez le lien connexe.
2. Spécifiez les éléments à exporter vers Excel en renseignant les champs. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Cliquez sur le bouton **OK**.

**Remarque :** le fichier Excel est doté des caractéristiques suivantes :

* Le solde est arrondi au point de pourcentage le plus proche, mais la valeur de la cellule indique le même pourcentage que dans les écritures comptables.

* Les nombres négatifs sont représentés comme des nombres positifs entre parenthèses. Par conséquent, -123 est représenté comme suit : (123).

## <a name="see-also"></a>Voir aussi
[Finance](finance-setup.md)   
[Configurer les processus financiers de base](finance-setup-setup-finance-setup.md)

