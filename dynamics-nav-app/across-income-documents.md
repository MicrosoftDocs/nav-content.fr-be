---
title: "Gérer les documents entrants"
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
ms.openlocfilehash: 49acc3549180b73dada6415f3ea40f17c1dd9e4c
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="manage-incoming-documents"></a>Gérer les documents entrants
Certaines transactions de société ne sont pas enregistrées dans Dynamics NAV dès le départ. À la place, un document provenant d'entreprise externe arrive dans votre société comme la pièce jointe d'un e-mail, ou une copie papier que vous pouvez scanner pour la classer. Cela est classique dans le cas des commandes, lorsque ces fichiers de documents entrants sont des reçus de paiements pour des dépenses ou de petits achats.

À partir de fichiers PDF ou image représentant des documents entrants, un service OCR externe (reconnaissance optique de caractères) peut générer des documents électroniques qui peuvent ensuite être convertis en enregistrements de document au sein de Dynamics NAV.

Dans la fenêtre **Documents entrants**, vous pouvez utiliser différentes fonctions pour examiner les reçus de dépenses, gérer les tâches ROC et convertir les fichiers document entrants, manuellement ou automatiquement, en documents ou lignes feuille appropriés. Les fichiers externes peuvent être joints à n'importe quelle étape du processus, notamment en ce qui concerne les documents validés et au fournisseur, au client qui en résulte, et dans les écritures comptables.

Le processus de document entrant est composé des activités principales suivantes :

* Enregistrez les documents externes dans Dynamics NAV en créant des lignes dans la fenêtre **Documents entrants** de l'une des manières suivantes :
    * Manuellement, à l'aide de fonctions simples, à partir d'un PC ou d'un périphérique mobile, de l'une des manières suivantes :
        * Utilisez le bouton **Créer à partir d'un fichier**, puis renseignez les champs appropriés dans la fenêtre **Document entrant**. Le fichier est automatiquement joint.  
        * Utilisez le bouton **Nouveau**, renseignez les champs appropriés dans la fenêtre **Document entrant**, puis joignez manuellement le fichier associé.
        * À partir d'une tablette ou d'un téléphone, utilisez le bouton **Créer à partir de l'appareil photo** pour créer un enregistrement de document entrant, puis envoyez l'image au service OCR, par exemple.
    * Automatiquement en recevant le document du service OCR en tant que document électronique après avoir envoyé par e-mail le fichier PDF ou image associé au service OCR. Le raccourci **Informations financières** est automatiquement renseigné dans la fenêtre **Document entrant**.
* Utilisez le service OCR pour convertir des fichiers PDF ou image en documents électroniques qui peuvent être convertis en enregistrements document dans Dynamics NAV.
* Créez des documents ou des lignes feuille comptabilité à partir d'enregistrements document entrants en saisissant les informations telles que vous les lisez à partir des fichiers document entrants.
* Joignez des fichiers document entrant à des documents vente et achat de tout statut, notamment au fournisseur, client, et écritures comptables qui résultent de la validation.
* Affichez les enregistrements document entrant et leurs pièces jointes à partir de tout document achat et vente ou de toute écriture, ou recherchez toutes les écritures comptables sans enregistrement document entrant dans la fenêtre **Plan comptable**.


|Pour |Voir |
|---|----|
|Configurer la fonctionnalité Documents entrants et le service OCR.|[Procédure : configurer les documents entrants](across-how-setup-income-documents.md)|
|Créer des enregistrements document entrant, joindre des fichiers, utiliser le service OCR pour convertir des fichiers PDF en documents électroniques, convertir les documents électroniques en enregistrements de document, auditer les enregistrements document entrant à partir de documents vente et achat validés.|[Traiter les documents entrants](across-process-income-documents.md)|

## <a name="see-also"></a>Voir aussi  
[Gestion des achats](purchasing-manage-purchasing.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

