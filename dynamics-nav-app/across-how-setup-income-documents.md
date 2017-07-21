---
title: "Procédure : configurer les documents entrants"
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
ms.openlocfilehash: 2bce97c76876c86a576ec6a281a306a46881027c
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-incoming-documents"></a>Procédure : configurer les documents entrants
Si vous créez des lignes feuille comptabilité à partir des enregistrements de documents entrants, vous devez spécifier dans la fenêtre **Paramètres des documents entrants** quels modèle et nom de feuille utiliser.

Si vous ne souhaitez pas que les utilisateurs créent des factures ou des lignes feuille comptabilité à partir d'enregistrements de documents entrants, sauf si les documents ont été préalablement approuvés, vous devez paramétrer des approbateurs dans la fenêtre **Approbateurs de document entrant**.

Pour convertir les fichiers PDF et image en documents électroniques que vous pouvez convertir, par exemple, en factures achat dans Dynamics NAV, vous devez d'abord configurer la fonctionnalité OCR et activer le service.

Une fois que la fonctionnalité Documents entrants est configurée, vous pouvez utiliser différentes fonctions pour examiner les reçus de dépenses, gérer les tâches ROC et convertir les fichiers document entrants, manuellement ou automatiquement, en documents ou lignes feuille appropriés. Les fichiers externes peuvent être joints à n'importe quelle étape du processus, notamment en ce qui concerne les documents validés et au fournisseur, au client qui en résulte, et dans les écritures comptables. Pour plus d'informations, reportez vous à [Procédure : traiter les documents entrants](across-process-income-documents.md).

## <a name="to-set-up-the-incoming-documents-feature"></a>Configurer la fonctionnalité Documents entrants
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Configuration document entrant**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

## <a name="to-set-up-approvers-of-incoming-document-records"></a>Configurer des approbateurs d'enregistrements document entrant
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Configuration document entrant**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Paramètres des documents entrants**, sélectionnez l'action **Approbateurs**.

    La fenêtre **Approbateurs de document entrant** affiche tous les utilisateurs configurés dans votre solution Dynamics NAV.  
3. Sélectionnez un ou plusieurs utilisateurs pouvant approuver un document entrant pour qu'un document ou une ligne feuille connexe puisse être créée.

Lorsque des approbateurs ont été configurés dans la fenêtre **Approbateurs de document entrant**, seuls ces utilisateurs peuvent approuver un document entrant si la case **Exiger une approbation pour créer** est cochée dans la fenêtre **Paramètres des documents entrants**.

**Remarque** : ce paramétrage d'approbation n'est pas lié aux flux d'approbation. Pour plus d'informations, reportez-vous à [Procédure : utilisation des flux d'approbation](across-how-use-approval-workflows.md).

## <a name="to-set-up-an-ocr-service"></a>Configurer un service ROC
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres service OCR**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.


## <a name="to-encrypt-your-login-information"></a>Chiffrer les informations de connexion
Il est recommandé de protéger les informations de connexion que vous saisissez dans la fenêtre **Paramètres service OCR**. Vous pouvez chiffrer des données sur le serveur en générant de nouvelles clés de chiffrement ou en important des clés existantes que vous activez sur l'instance de serveur qui est connectée à la base de données.

1. Dans la fenêtre **Paramètres service OCR**, sélectionnez l'action **Gestion du chiffrement**.
2. Dans la fenêtre **Gestion du chiffrement des données**, activez le chiffrement de vos données.

## <a name="see-also"></a>Voir aussi  
[Traiter les documents entrants](across-process-income-documents.md)  
[Documents entrants](across-income-documents.md)  
[Gestion des achats](purchasing-manage-purchasing.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

