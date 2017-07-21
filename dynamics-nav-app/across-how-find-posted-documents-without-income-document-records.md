---
title: "Procédure : Rechercher des enregistrements validés sans enregistrements document entrant"
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
ms.openlocfilehash: eb65922decc86ca6834cae4cf46c6f2ff492e29c
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-find-posted-documents-without-incoming-document-records"></a>Procédure : Rechercher des enregistrements validés sans enregistrements document entrant
Depuis les fenêtres **Plan comptable** et **Écritures comptables**, vous pouvez utiliser la fonction de recherche pour rechercher les écritures comptables pour des documents achat et vente validés qui n'ont pas d'enregistrement de document entrant, puis les lier de façon centralisée à des enregistrements existants ou en créer de nouveaux avec des fichiers joints.

## <a name="to-find-posted-documents-without-incoming-document-records"></a>Rechercher des enregistrements validés sans enregistrements document entrant
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Plan comptable**, puis sélectionnez le lien connexe.
2. Sélectionnez une ligne pour un compte général pour les écritures comptables duquel vous souhaitez voir les documents ventes et achats validés sans enregistrement document entrant, puis sélectionnez l'action **Documents validés sans document entrant**.
3. Sinon, sélectionnez l'action **Écritures comptables**.
4. Dans la fenêtre **Écritures comptables**, sélectionnez l'action **Documents validés sans documents entrants**.

La fenêtre **Documents validés sans document entrant** s'ouvre et affiche des documents achat et vente validés sans enregistrement document entrant représenté par des écritures comptables du compte général pour lequel vous avez ouvert la fenêtre. Au maximum, la fenêtre affiche 1 000 lignes. Par défaut, le champ **Filtre date** contient donc un filtre qui limite l'affichage des lignes à celles dont les écritures ont une date comptabilisation comprise entre le début de la période comptable et la date de travail.

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a>Lier des documents recherchés à des enregistrements document entrant existants
1. Dans la fenêtre **Documents validés sans document entrant**, sélectionnez la ligne d'un document valisé que vous souhaitez lier à un enregistrement document entrant existant, puis sélectionnez l'action **Sélectionner le document entrant**.
2. Dans la fenêtre **Documents entrants**, sélectionnez l'enregistrement document entrant que vous souhaitez lier au document validé trouvé, puis sélectionnez le bouton **OK**.
3. Dans la fenêtre **Documents validés sans document entrant**, l'enregistrement document entrant sélectionné est désormais lié au document validé, comme vous pouvez le constater dans le récapitulatif **Fichiers du document entrant**.

Si un enregistrement document entrant approprié n'existe pas dans la fenêtre **Documents entrants**, vous pouvez le créer. Pour plus d'informations, reportez vous à [Procédure : créer des enregistrements document entrant](across-how-create-income-document-records.md).

## <a name="see-also"></a>Voir aussi  
[Traiter les documents entrants](across-process-income-documents.md)  
[Documents entrants](across-income-documents.md)  
[Gestion des achats](purchasing-manage-purchasing.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

