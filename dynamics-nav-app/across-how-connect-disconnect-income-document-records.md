---
title: "Procédure : connecter et déconnecter des enregistrements document entrant à partir de documents et d'écritures"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: fece4e6e38075db6d394c71418fda82a7aa082e1
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-connect-and-disconnect-incoming-document-records-from-documents-and-entries"></a>Procédure : connecter et déconnecter des enregistrements document entrant à partir de documents et d'écritures
Vous pouvez stocker des documents professionnels externes dans Dynamics NAV en joignant les fichiers document aux enregistrements document entrant connexes. Si le document, une facture achat par exemple, n'était pas dès le départ un enregistrement document entrant, vous pouvez toujours créer et le lier à un enregistrement document entrant ultérieurement. Vous pouvez également joindre des fichiers document entrant à des documents achat et vente validés et à des écritures fournisseur, client et comptables à l'aide du récapitulatif **Fichiers document entrant** dans, par exemple, les fenêtres **Factures achat enregistrées** et **Écritures comptables fournisseur**.

Depuis les fenêtres **Plan comptable** et **Écritures comptables**, vous pouvez utiliser la fonction de recherche pour rechercher les écritures comptables pour des documents achat et vente validés qui n'ont pas d'enregistrement de document entrant, puis les lier de façon centralisée à des enregistrements existants ou en créer de nouveaux avec des fichiers joints. Pour plus d'informations, reportez-vous à [Procédure : Rechercher des enregistrements validés sans enregistrements document entrant](across-how-find-posted-documents-without-income-document-records.md).

Les procédures suivantes indiquent comment joindre un fichier à une facture achat existante qui n'a pas été créée à partir d'un enregistrement document entrant et comment joindre un fichier à une écriture comptable fournisseur. La même action permet de joindre un fichier à des documents achat ou vente validés.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a>Créer et lier un enregistrement document entrant à partir d'une facture achat
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Factures achat**, puis sélectionnez le lien connexe.
2. Sélectionnez la ligne de la facture achat à laquelle vous souhaitez joindre un fichier, puis sélectionnez l'action **Créer un document entrant à partir d'un fichier**.
3. Vous pouvez également sélectionner la ligne de la facture achat à laquelle vous souhaitez joindre un fichier, puis sélectionner l'action **Joindre fichier**.
4. Dans la fenêtre **Insérer un fichier**, sélectionnez le fichier qui représente le document entrant concerné, puis choisissez le bouton **Ouvrir**.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a>Créer et lier un enregistrement document entrant à partir d'une écriture comptable fournisseur
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Écritures comptables fournisseur**, puis sélectionnez le lien connexe.
2. Sélectionnez une ligne d'une écriture comptable fournisseur à laquelle vous souhaitez joindre un fichier, puis sélectionnez l'action **Créer un document entrant à partir d'un fichier**.
3. Vous pouvez également sélectionner une ligne d'une une écriture comptable fournisseur à laquelle vous souhaitez joindre un fichier, puis sélectionner l'action **Joindre fichier**.
4. Dans la fenêtre **Insérer un fichier**, sélectionnez le fichier qui représente le document entrant concerné, puis choisissez le bouton **Ouvrir**.

## <a name="to-remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a>Pour supprimer la connexion d'un enregistrement document entrant à un document validé
Vous pouvez supprimer des fichiers joints de documents non validés à tout moment en supprimant l'enregistrement document entrant associé. Si le document est validé, vous devez d'abord supprimer la connexion de l'enregistrement document entrant.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Documents entrants**, puis sélectionnez le lien connexe.
2. Sélectionnez la ligne correspondant à un enregistrement document entrant lié à un document validé que vous souhaitez supprimer, puis sélectionnez **Supprimer la référence à l'enregistrement**.

La connexion au document validé est supprimée. Vous pouvez maintenant connecter un autre enregistrement document entrant au document validé, comme cela est décrit dans cette rubrique.

## <a name="see-also"></a>Voir aussi  
[Traiter les documents entrants](across-process-income-documents.md)  
[Documents entrants](across-income-documents.md)  
[Gestion des achats](purchasing-manage-purchasing.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

