---
title: "Procédure : Rapprocher les paiements à l'aide de l'application automatique"
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
ms.openlocfilehash: bde263424bb8e5b60d2c9a139ddc8bfef0a90062
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-payments-using-automatic-application"></a>Procédure : Rapprocher les paiements à l'aide de l'application automatique
La fenêtre **Feuille rapprochement bancaire** spécifie les paiements (entrants ou sortants) qui ont été enregistrés en tant que transactions sur votre compte bancaire en ligne et que vous pouvez lettrer à leurs écritures comptables ouvertes client, fournisseur et compte bancaire. Vous renseignez les lignes de la feuille en important un relevé bancaire sous forme de fichier ou flux bancaire.

Une feuille rapprochement bancaire est associée à un compte bancaire dans Dynamics NAV, qui reflète le compte bancaire en ligne sur lequel les transactions de paiement sont validées. Toutes les écritures comptables compte bancaire ouvertes associées au client lettré ou à des écritures comptables fournisseur sont clôturées lorsque vous sélectionnez l'action **Valider les paiements et rapprocher les comptes bancaires**. Cela signifie que le compte bancaire est automatiquement rapproché pour les paiements que vous validez avec le journal.

Si vous souhaitez importer des relevés bancaires en tant que flux bancaires, vous devez d'abord activer le service de flux de la Envestnet Yodlee Bank, puis associer le compte bancaire au compte bancaire en ligne associé. La feuille rapprochement bancaire détectera alors automatiquement les flux bancaire si vous sélectionnez l'action **Importer les transactions bancaires**. En outre, vous pouvez définir un compte bancaire de sorte à importer automatiquement de nouveaux flux de relevés bancaires toutes les heures. Les transactions pour les paiements qui ont déjà été validés comme lettrés et/ou rapprochés ne sont pas importées. Pour plus d'informations, reportez-vous à [Procédure: configurer le service de flux de la Envestnet Yodlee Bank](bank-how-setup-bank-statement-service.md).

**Remarque** : le service Envestnet Yodlee Bank Feeds, ou tout service de flux bancaire d'un autre fournisseur, risque de ne pas être disponible dans votre système. Contactez votre partenaire Microsoft si vous souhaitez utiliser un service de flux bancaire pour importer les relevés bancaires.

L'action **Mapper le texte avec le compte** vous permet de configurer des mappages entre le texte des paiements et des comptes de débit, de crédit et de contrepartie spécifiques afin que ces paiements soient validés dans les comptes spécifiés lorsque vous validez la feuille rapprochement bancaire. Reportez-vous à l'étape 9. Pour plus d'informations, reportez-vous à [Procédure : mapper du texte sur les paiements récurrents aux comptes pour un rapprochement automatique](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

Une fonctionnalité similaire existe pour rapprocher les montants en excédent sur les lignes feuille rapprochement bancaire de façon ponctuelle. Pour plus d'informations, reportez-vous à [Procédure : rapprocher les paiements qui ne peuvent pas être lettrés](receivables-how-reconcile-payments-cannot-apply-auto.md).

Vous utilisez la fonction **Lettrer automatiquement**, soit automatiquement lorsque vous importez un fichier ou flux bancaire avec transactions de paiement ou lorsque vous l'activez, pour lettrer des paiements à leurs écritures ouvertes associées sur la base d'une correspondance entre les données d'une ligne feuille et celles d'une ou plusieurs écritures ouvertes.

Sur les lignes feuille dans lesquelles un paiement a été lettré automatiquement à une ou plusieurs écritures ouvertes, le champ **Fiabilité correspondance** présente une valeur entre Faible et Élevée pour indiquer la qualité de la correspondance des données sur laquelle le lettrage de paiement suggéré est basée. En outre, les champs **Type compte** and **N° compte** sont renseignés avec les informations sur le client ou le fournisseur auquel le paiement validé est lettré. Si vous définissez un mappage de texte à compte, le lettrage automatique peut entraîner une valeur de fiabilité de correspondance **Élevée – Mappage de texte à compte**.

Pour chaque ligne feuille de la fenêtre **Feuille rapprochement bancaire**, vous pouvez ouvrir la fenêtre **Lettrage paiement** pour visualiser toutes les écritures ouvertes candidates au paiement et pour afficher les informations détaillées pour chaque écriture sur la correspondance des données sur laquelle un lettrage de paiement est basé. Ici, vous pouvez appliquer les paiements manuellement ou réappliquer les paiements qui ont été automatiquement appliqués à une écriture incorrecte. Pour plus d'informations, reportez-vous à [Procédure : réviser ou lettrer les paiements après application automatique](receivables-how-review-apply-payments-auto-application.md).

**Remarque** : vous pouvez lancer l'importation des transactions bancaires en même temps que vous ouvrez la fenêtre **Feuille rapprochement bancaire** pour une feuille rapprochement bancaire existante dans la fenêtre **Feuilles rapprochement bancaire**. La procédure suivante décrit comment importer des transactions bancaires dans la fenêtre **Feuille rapprochement bancaire** après avoir créé une nouvelle feuille.

## <a name="to-reconcile-payments-using-automatic-application"></a>Pour rapprocher les paiements à l'aide du lettrage automatique
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuilles rapprochement bancaire**, puis sélectionnez le lien connexe.
2. Pour travailler dans une nouvelle feuille rapprochement bancaire, sélectionnez l'action **Nouvelle feuille**.
3. Dans la fenêtre **Liste comptes bancaires paiement**, sélectionnez le compte bancaire pour lequel vous voulez rapprocher des paiements, puis cliquez sur le bouton **OK**.
La fenêtre **Feuille rapprochement bancaire** s'ouvre préparée pour le compte bancaire sélectionné.
4. Choisissez l'action **Importer les transactions bancaires**.
Si le compte bancaire pour la feuille sélectionnée n'est pas configuré pour importer des transactions bancaires, alors une boîte de dialogue s'ouvre pour vous aider à renseigner les champs appropriés.
5. Dans la fenêtre **Sélectionner un fichier à importer**, sélectionnez le fichier contenant les transactions bancaires pour les paiements que vous souhaitez rapprocher, puis cliquez sur le bouton **Ouvrir**.  
6. Si le service de relevé bancaire est activé, dans la fenêtre **Filtre de relevé bancaire** qui s'ouvre automatiquement, spécifiez l'intervalle de temps pour l'importation des relevés bancaires.

    La fenêtre **Feuille rapprochement bancaire** est renseignée avec les lignes pour les paiements représentant les transactions bancaires dans le relevé bancaire importé.

    Sur les lignes pour les paiements qui ont été automatiquement lettrés à leurs écritures ouvertes associées, le champ **Fiabilité correspondance** présente une valeur entre **Faible** et **Élevée** pour indiquer la qualité de la correspondance des données sur laquelle le lettrage du paiement suggéré est basé. En outre, les champs **Type compte** and **N° compte** sont renseignés avec les informations sur le client ou le fournisseur auquel le paiement validé est lettré.
7. Sélectionnez une feuille journal, puis sélectionnez l'action **Lettrer manuellement** pour réviser, relettrer ou lettrer le paiement manuellement dans la fenêtre **Lettrage paiement**. Pour plus d'informations, reportez-vous à [Procédure : réviser ou lettrer les paiements après application automatique](receivables-how-review-apply-payments-auto-application.md).

    Une fois le lettrage manuel terminé, le champ **Fiabilité correspondance** de la ligne feuille que vous avez traitée manuellement contient la valeur **Accepté**.
8. Sélectionnez une ligne feuille non lettrée pour une réception ou une dépense récurrente en liquide, par exemple l'achat de carburant pour une voiture, puis sous l'onglet Accueil du groupe Vérifier, sélectionnez Mapper le texte avec le compte. Pour plus d'informations, reportez-vous à [Procédure : mapper du texte sur les paiements récurrents aux comptes pour un rapprochement automatique](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).
9. Une fois terminé le mappage du texte de paiement avec les comptes, sélectionnez l'action **Lettrer manuellement**.
10. Lorsque vous êtes certain que tous les paiements sur les lignes feuille sont correctement lettrés ou définis sur la comptabilisation directe, sélectionnez l'action **Valider**.

Lorsque vous validez la feuille de rapprochement de paiements, les écritures ouvertes appliquées sont clôturées et les comptes client, fournisseur ou généraux liés sont mis à jour. Pour les paiements sur les lignes feuille basées sur le mappage de texte à compte, les comptes généraux, client et fournisseur spécifiés sont mis à jour. Pour toutes les lignes feuille, des écritures comptables compte bancaire sont créées. Si vous sélectionnez l'action **Valider les paiements et rapprocher les comptes bancaires**, toutes les écritures comptables compte bancaire ouvertes associées au client lettré ou à des écritures comptables fournisseur sont clôturées. Cela signifie que le compte bancaire est automatiquement rapproché pour les paiements que vous validez avec le journal.

Vous pouvez comparer la valeur du champ **Solde sur compte bancaire après validation** avec la valeur du champ **Solde final du relevé** pour avoir un suivi lorsque le compte bancaire a fait l'objet d'un rapprochement en fonction des paiements que vous validez.

**Remarque** : si vous ne souhaitez pas rapprocher le compte bancaire à partir de la fenêtre **Feuille rapprochement bancaire**, vous devez utiliser la fenêtre **Rapprochement bancaire**. Pour plus d'informations, reportez vous à [Rapprocher des comptes bancaires séparément](bank-how-reconcile-bank-accounts-separately.md).

## <a name="see-also"></a>Voir aussi
[Gestion des comptes client](receivables-manage-receivables.md)  
[Gestion des ventes](sales-manage-sales.md)

