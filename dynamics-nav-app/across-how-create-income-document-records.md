---
title: "Procédure : créer des enregistrements document entrant"
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
ms.openlocfilehash: 10ba191b197be8b98b2d5d5ab9ac4bc3baf0d82b
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-create-incoming-document-records"></a>Procédure : créer des enregistrements document entrant
Dans la fenêtre **Documents entrants**, vous pouvez utiliser différentes fonctions pour examiner les reçus de dépenses, gérer les tâches ROC et convertir les fichiers document entrants, manuellement ou automatiquement, en documents ou lignes feuille appropriés. Les fichiers externes peuvent être joints à n'importe quelle étape du processus, notamment en ce qui concerne les documents validés et au fournisseur, au client qui en résulte, et dans les écritures comptables.

Pour enregistrer un document externe dans Dynamics NAV, vous devez d'abord créer ou terminer un enregistrement document entrant. Vous pouvez effectuer cette opération manuellement ou prendre une photo du document externe puis créer l'enregistrement document entrant avec le fichier image joint.

Avant d'utiliser la fonctionnalité Documents entrants, vous devez exécuter la configuration requise. Pour plus d'informations, reportez vous à [Procédure : configurer des documents entrants](across-how-setup-income-documents.md).

## <a name="to-approve-or-reject-an-incoming-document"></a>Approbation ou rejet d'un document entrant
Si vous souhaitez autoriser des utilisateurs à créer des factures ou des lignes feuille comptabilité à partir d'enregistrements document entrant, sauf s'ils sont approbateurs, vous pouvez configurer des approbateurs qui doivent approuver les enregistrements avant de pouvoir être traités.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Documents entrants**, puis sélectionnez le lien connexe.
2. Sélectionnez la ligne contenant le document à approuver ou rejeter, puis sélectionnez l'action **Approuver** or **Rejeter**.

Si vous approuvez l'enregistrement document entrant, la case à cocher **Lancé** de la ligne document entrant est activée. L'utilisateur chargé de créer, par exemple, des factures achat peut continuer à traiter l'enregistrement.

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a>Pour créer un enregistrement de document entrant en prenant une photo
**Remarque** : la procédure suivante s'applique uniquement aux tablettes et téléphones clients Dynamics NAV.

1. Dans la barre d'application, sélectionnez la mosaïque **Créer le document entrant à partir de l'appareil photo**, puis passez à l'étape 4.
2. Sinon, dans la barre d'application, cliquez sur le bouton Options, choisissez **Documents entrants**, puis **Tous**.
3. Dans la fenêtre **Documents entrants**, sélectionnez le bouton de sélection, puis **Créer à partir de l'appareil photo**. L'appareil photo de la tablette ou du téléphone est activé.
4. Prenez une photo d'un document, tel qu'un reçu d'achat, que vous souhaitez traiter en tant que document entrant, puis sélectionnez le bouton **OK**.

Un enregistrement de document entrant est créé, avec l'image jointe.

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a>Pour joindre une image à un enregistrement de document entrant en prenant une photo
**Remarque** : la procédure suivante s'applique uniquement aux tablettes et téléphones clients Dynamics NAV.

1. Dans la barre d'application, cliquez sur le bouton Options, choisissez **Documents entrants**, puis **Tous**.
2. Ouvrez la fiche de l'enregistrement de document entrant existant.
3. Dans la fenêtre **Document entrant**, sélectionnez le bouton de sélection, puis **Joindre l'image de l'appareil photo**. L'appareil photo de la tablette ou du téléphone est activé.
4. Prenez une photo d'un document, tel qu'un reçu d'achat, que vous souhaitez traiter en tant que document entrant, puis sélectionnez le bouton **OK**.

L'image est jointe à l'enregistrement de document entrant.

## <a name="to-create-an-incoming-document-record-manually"></a>Pour créer un enregistrement document entrant manuellement
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Documents entrants**, puis sélectionnez le lien connexe.
2. Choisissez l'action **Créer à partir d'un fichier**.  
3. Dans la fenêtre **Insérer un fichier**, sélectionnez un fichier, puis choisissez **Ouvrir**.

    Le fichier est automatiquement joint.
4. Sinon, choisissez l'action **Nouveau**.
5. Pour joindre un fichier, choisissez l'action **Joindre fichier**.
6. Dans la fenêtre **Insérer un fichier**, sélectionnez le fichier qui représente le document entrant concerné, puis choisissez le bouton **Ouvrir**.
7. Dans la fenêtre **Document entrant**, renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

##<a name="see-also"></a>Voir aussi  
[Traiter les documents entrants](across-process-income-documents.md)  
[Documents entrants](across-income-documents.md)  
[Gestion des achats](purchasing-manage-purchasing.md)  
[Utiliser Dynamics NAV](ui-work-product.md)
