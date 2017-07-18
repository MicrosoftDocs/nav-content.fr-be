---
title: "Procédure d'exportation de paiements vers un fichier bancaire"
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
ms.openlocfilehash: 09bdf56b3d5e76b12d868091e89232ce9c08e215
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-export-payments-to-a-bank-file"></a>Procédure d'exportation de paiements vers un fichier bancaire
Lorsque vous êtes prêt à effectuer des paiements à vos fournisseurs par l'intermédiaire de la fenêtre **Feuille paiement**, vous pouvez exporter un fichier contenant les informations de paiement sur les lignes feuille. Vous pouvez ensuite transférer le fichier à votre banque électronique qu'elle traite les transferts d'argent associés.

Dans la version générique de Dynamics NAV, un fournisseur global de services pour convertir les données bancaires dans n'importe quel format de fichier que votre banque requiert est paramétré et connecté.

**Remarque** : pour pouvoir exporter à partir d'une feuille paiement, vous devez activer le champ exporter dans la feuille associée. En outre, votre compte bancaire et le compte bancaire du fournisseur doivent être paramétrés pour le paiement électronique. Pour plus d'informations, reportez-vous à [Procédure: configurer le service de conversion de données bancaires](bank-how-setup-bank-data-conversion-service.md).

La fenêtre **Registres virement** vous permet d'afficher les fichiers paiement qui ont été exportés de la feuille paiement. A partir de cette fenêtre, vous pouvez également réexporter des fichiers paiement en cas d'erreurs techniques ou de modifications des fichiers.

## <a name="to-export-payments-to-a-bank-file"></a>Pour exporter des paiements vers un fichier bancaire
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuilles paiement**, puis sélectionnez le lien connexe.
2. Remplissez les lignes feuille paiement, par exemple à l'aide de la fonction **Proposer paiements fournisseur**. Pour plus d'informations, reportez vous à [Procédure : proposer des paiements fournisseur](payables-how-suggest-vendor-payments.md).  
3. Lorsque vous avez renseigné toutes les lignes feuille paiement, sélectionnez **Exporter le paiement vers un fichier**.

    Chaque message d'erreur est affiché dans le récapitulatif **Erreurs fichier de paiement** dans lequel vous pouvez également choisir un message d'erreur pour afficher les informations détaillées. Vous devez résoudre toutes les erreurs avant que le fichier de paiement ne puisse être exporté.

    **Conseil**: lorsque vous utilisez le service conversion données bancaires, un message d'erreur courant stipule que le numéro de compte bancaire n'a pas la longueur requise par votre banque. Pour éviter ou résoudre l'erreur, vous devez supprimer la valeur du champ **IBAN** de la fenêtre **Fiche compte bancaire** puis, dans le champ **N° compte bancaire**, saisissez un numéro de compte bancaire au format exigé par votre banque.
4. Dans la fenêtre **Enregistrer sous**, spécifiez l'emplacement où le fichier est exporté, puis choisissez **Enregistrer**.

Le fichier de paiement bancaire est exporté à l'emplacement que vous spécifiez et vous pouvez passer à son téléchargement sur votre compte bancaire électronique et effectuer les paiements.

Lorsque vous recevez la confirmation que les paiements sont traités avec succès dans la banque, vous pouvez valider les lignes feuille paiement exportées.

## <a name="to-plan-when-to-post-exported-payments"></a>Pour planifier la validation des paiements exportés
Si vous ne souhaitez pas valider une ligne feuille paiement pour un paiement exporté, par exemple parce que vous attendez la confirmation que la transaction a été traitée par la banque, vous pouvez simplement supprimer la ligne feuille. Lorsque vous créez ensuite une ligne feuille paiement pour payer le montant ouvert de la facture, le champ **Montant total exporté** affiche la quantité du montant ayant déjà été exportée. En outre, vous pouvez rechercher des informations détaillées concernant le total exporté en cliquant sur le bouton **Écritures reg. virement** pour visualiser des détails sur les fichiers de paiement exportés.

Si vous appliquez un processus selon lequel vous ne validez pas les paiements tant que vous n'avez pas la confirmation qu'ils ont été traités par la banque, vous pouvez contrôler ceci de deux façons.

* Dans une feuille paiement avec les lignes paiement proposées, vous pouvez trier soit la colonne **Exporté dans fichier paiement** soit la colonne **Montant total exporté**, puis supprimer les propositions de paiement pour les factures ouvertes pour lesquelles les paiements ont déjà été effectués et pour lesquelles vous ne souhaitez pas effectuer de paiements.
* Dans la fenêtre **Proposer paiements fournisseur**, où vous spécifiez les paiements à insérer dans la feuille de paiement, vous pouvez cochez la case **Ignorer les paiements exportés** si vous ne souhaitez pas insérer des lignes feuille pour les paiements qui ont déjà été exportés.

Pour afficher des informations sur les paiements exportés, sélectionnez l'action **Historique d'exportation des paiements**.

## <a name="to-re-export-payments-to-a-bank-file"></a>Pour réexporter des paiements vers un fichier bancaire
Vous pouvez réexporter des fichiers paiement à partir de la fenêtre **Registres virement**. Avant de supprimer ou de valider les lignes feuille paiement, vous pouvez également réexporter le fichier de paiement à partir de la fenêtre **Feuille paiement** en l'exportant simplement à nouveau.

Si vous avez supprimé ou validé les lignes feuille paiement après les avoir exportées, vous pouvez réexporter le même fichier de paiement à partir de la fenêtre **Registres virement**. Sélectionnez la ligne correspondant au lot de virements que vous souhaitez réexporter, puis, sélectionnez l'action **Réexporter les paiements dans un fichier**.

## <a name="see-also"></a>Voir aussi
[Fournisseurs](payables-manage-payables.md)  
[Gestion des achats](purchasing-manage-purchasing.md)  
[Configuration des procédures achat](purchasing-setup-purchasing.md)

