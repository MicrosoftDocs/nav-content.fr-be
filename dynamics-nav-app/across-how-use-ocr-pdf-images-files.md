---
title: "Procédure : Utiliser un service OCR pour convertir des fichiers PDF et image en documents électroniques"
author: SorenGP
ms.custom: na
ms.date: 10/06/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 96b1baf3554d3647e75223bb4cb1ee08dc21eb6d
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-ocr-to-turn-pdf-and-image-files-into-electronic-documents"></a>Procédure : Utiliser un service OCR pour convertir des fichiers PDF et image en documents électroniques
À partir de fichiers PDF ou image reçus de vos partenaires commerciaux, un service externe de reconnaissance optique de caractères (OCR) génère des documents électroniques qui peuvent être convertis en enregistrements document dans Dynamics NAV. Par exemple, lorsque vous recevez une facture au format PDF de votre fournisseur, vous pouvez l'envoyer au service OCR à partir de la fenêtre **Documents entrants**. Ceci est décrit dans la première procédure.

Au lieu d'envoyer le fichier depuis la fenêtre **Documents entrants**, vous pouvez l'envoyer au service OCR par e-mail. Ensuite, lorsque vous recevez le document électronique, un enregistrement de document entrant associé est créé automatiquement. Ceci est décrit dans la deuxième procédure.

Après quelques secondes, vous recevrez le fichier du service OCR en tant que facture électronique pouvant être convertie en facture achat pour le fournisseur. Ceci est décrit dans la troisième procédure.

Comme le service OCR est basé sur la reconnaissance optique, il est probable qu'il interprète de manière incorrecte les caractères des fichiers PDF ou image lorsqu'il traite pour la première fois les documents d'un fournisseur donné, par exemple. Il peut ne pas interpréter le logo de la société comme le nom du fournisseur ou il peut mal interpréter le montant total sur un reçu en raison de sa disposition. Pour éviter ces erreurs à l'avenir, vous pouvez les corriger dans une version distincte de la fenêtre **Document entrant**. Vous envoyez ensuite les corrections au service OCR de manière à ce qu'il interprète correctement les caractères spécifiques la prochaine fois qu'il traite un document PDF ou image pour le même fournisseur. Pour plus d'informations, reportez-vous à la section « Former le service OCR afin d'éviter des erreurs ».

Le trafic des fichiers entrants et sortants du service OCR est traité par une écriture de la file projets dédiée, qui est créée automatiquement lorsque vous activez la connexion au service correspondant. Pour plus d'informations, reportez vous à [Procédure : configurer des documents entrants](across-how-setup-income-documents.md).

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-from-the-incoming-documents-window"></a>Pour envoyer un fichier PDF ou image au service OCR à partir de la fenêtre **Documents entrants**
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Documents entrants**, puis sélectionnez le lien connexe.
2. Créez un enregistrement de document entrant et joignez le fichier. Pour plus d'informations, reportez vous à [Procédure : créer des enregistrements document entrant](across-how-create-income-document-records.md).  
3. Dans la fenêtre **Documents entrants**, sélectionnez une ou plusieurs lignes, puis sélectionnez l'action **Envoyer à la file d'attente des travaux**.

    La valeur dans le champ **Statut OCR** passe à **Prêt**. Le fichier PDF ou image joint est envoyé au service OCR par la file projets en fonction du planning, à condition qu'il n'existe aucune erreur.
5. Sinon, dans la fenêtre **Documents entrants**, sélectionnez une ou plusieurs lignes, puis sélectionnez l'action **Envoyer au service OCR**.

La valeur du champ **Statut OCR** passe à Envoyé, à condition qu'il n'existe aucune erreur.

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-by-email"></a>Pour envoyer un fichier PDF ou image au service OCR par e-mail
À partir de votre application de messagerie, vous pouvez envoyer un e-mail au fournisseur de service OCR en joignant le fichier PDF ou image. Pour plus d'informations sur l'adresse e-mail d'envoi, reportez-vous au site Web du fournisseur de service OCR.

Puisqu'aucun enregistrement de document entrant n'existe pour le fichier, un enregistrement est automatiquement créé dans la fenêtre **Documents entrants** lorsque vous recevez le document électronique du service OCR. Pour plus d'informations, reportez vous à [Procédure : créer des enregistrements document entrant](across-how-create-income-document-records.md).

**Remarque** : Si vous utilisez une tablette ou un téléphone, vous pouvez envoyer le fichier au service OCR dès que vous avez pris une photo du document, ou vous pouvez créer un document entrant directement. Pour plus d'informations, voir la section « Créer des enregistrements document entrants en prenant une photo » dans [Procédure : créer des enregistrements document entrants](across-how-create-income-document-records.md).

## <a name="to-receive-the-resulting-electronic-document-from-the-ocr-service"></a>Réceptionner le document électronique résultant du service ORC.
Le document électronique qui est créé par le service OCR à partir du fichier PDF ou image est automatiquement réceptionné dans la fenêtre **Documents entrants** par l'entrée de la file d'attente des travaux qui est configurée lorsque vous activez le service OCR.

Si vous n'utilisez pas de file d'attente des travaux, ou si vous souhaitez recevoir un document OCR finalisé avant l'échéance indiquée par la file d'attente des travaux, vous pouvez choisir le bouton **Recevoir du service OCR**. Cela vous permettra d'obtenir tous les documents finalisés par le service OCR.

**Remarque**: si le service OCR est configuré de telle façon qu'une vérification manuelle des documents traités est exigée, le champ **Statut OCR** affichera donc **En attente de vérification**. Dans ce cas, procédez comme suit pour vous connecter au site Web du service OCR et vérifier manuellement un document OCR.

1. Dans le champ **Statut OCR**, sélectionnez le lien hypertexte **En attente de vérification**. Sinon, optez pour la mosaïque **En attente de vérification** de la page d'accueil.
2. Sur le site Web du service OCR, connectez-vous à l'aide des identifiants de votre compte de service OCR. Il s'agit des identifiants que vous avez également utilisés lors de la configuration de ce service. Pour en savoir plus, consultez la section « Configurer un service OCR » dans [Procédure : configurer les documents entrants](across-how-setup-income-documents.md).

    Si vous accédez au site Web à partir du champ **Statut OCR**, le document en question s'affiche immédiatement après votre connexion. Si vous accédez au site Web en sélectionnant la mosaïque de la page d'accueil, sur la première page du service OCR qui s'ouvre, vous devez choisir le bouton **Démarrer** sur l'onglet **Vérifier** ou double-cliquer sur le document que vous souhaitez vérifier.

    Les informations concernant le document OCR sont affichées, vous présentant à la fois le contenu source du fichier PDF ou image ainsi que les valeurs de champ OCR correspondantes.
3. Examinez les différentes valeurs de champ et modifiez ou saisissez des valeurs dans les champs identifiés comme à vérifier par le service OCR.
4. Cliquez sur le bouton **OK**. Le processus OCR est terminé et le document électronique résultant est envoyé à la fenêtre **Documents entrants** dans Dynamics NAV, selon l'échéance de la file d'attente des travaux.

    Si vous accédez au site Web en sélectionnant la mosaïque de la page d'accueil, tout autre document OCR à vérifier est automatiquement affiché sur le site Web.
5. Répétez l'étape 4 pour tout autre document OCR à vérifier.

Désormais, vous pouvez poursuivre la création d'enregistrements de documents pour les documents électroniques reçus dans Dynamics NAV, manuellement ou automatiquement. Pour en savoir plus, voir la section « Créer un enregistrement de document dans Dynamics NAV à partir d'un document OCR reçu ». Vous pouvez également connecter le nouvel enregistrement document entrant au document existant validé ou non validé de telle sorte que le fichier source soit facile d'accès à partir de Dynamics NAV. Pour plus d'informations, voir la section [Traiter les documents entrants](across-process-income-documents.md).

## <a name="to-create-a-purchase-invoice-from-an-electronic-document-received-from-the-ocr-service"></a>Pour créer une facture achat à partir d'un document électronique réceptionné depuis le service OCR
La procédure suivante décrit comment créer un enregistrement facture achat à partir d'une facture fournisseur reçue en pièce jointe provenant du service OCR. La procédure est identique lorsque vous créez, par exemple, une ligne feuille comptabilité à partir d'un justificatif de frais.

**Remarque**: les champs **Description** et **N°** des lignes document créées ne seront pas complétées tant que vous n'aurez pas mappé tout d'abord le texte trouvé sur le document OCR avec les deux champs dans Dynamics NAV. Vous pouvez le faire en tant que références externes article, pour les lignes document de type Article, ou en tant que mappages de texte à compte, pour les lignes document ou les feuilles comptabilité de type Compte général. Pour en savoir plus, voir l'info-bulle pour l'action **Références externes** sur les fiches article et la procédure associée [Procédure : mapper le texte sur les paiements récurrents vers les comptes pour rapprochement automatique](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

Pour les documents entrants, vous utilisez généralement l'action **Mapper le texte avec le compte** pour définir qu'un certain texte sur une facture fournisseur en provenance du service OCR est mappé avec un certain compte fournisseur. En outre, toute partie de la description du document entrant qui existe comme texte de mappage signifie que le champ **N°** sur le document résultant ou les lignes feuille de type Compte général sont complétées par le fournisseur en question.

Outre le mappage avec un compte fournisseur ou des comptes généraux, vous pouvez également effectuer un mappage avec un compte bancaire. Ceci est utile, par exemple, pour les documents électroniques des dépenses qui sont déjà payées lorsque vous souhaitez créer une ligne feuille comptabilité qui est prête à être validée sur un compte bancaire.

1. Sélectionnez la ligne document entrant pour le document électronique fournisseur provenant du service OCR.
2. Pour mapper le texte sur le document avec le compte Fournisseur, compte de débit, sélectionnez l'action **Mapper le texte avec le compte**, puis complétez la fenêtre **Mappage de texte à compte** avec les informations qui s'appliqueront, par la suite, au fournisseur. Pour plus d'informations, reportez-vous à [Procédure : mapper du texte sur les paiements récurrents aux comptes pour un rapprochement automatique](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).
3. Pour mapper les numéros d'article sur le document avec vos descriptions des articles du fournisseur, ouvrez la fiche de chaque article, puis choisissez l'action **Références externes** afin de configurer les références externes entre vos descriptions d'article et celles du fournisseur.
4. Dans la fenêtre **Documents entrants**, sélectionnez l'action **Créer un document**.

Une facture achat sera créée dans Dynamics NAV selon les informations disponibles sur le document électronique du fournisseur provenant du service OCR.

Les erreurs de validation, généralement associées à des données de base erronées ou manquantes dans Dynamics NAV, seront affichées sur le raccourci **Erreurs et avertissements**. Pour plus d'informations, reportez-vous à la section « Gérer les erreurs lors de la réception de documents électroniques ».

## <a name="to-handle-errors-when-receiving-electronic-documents"></a>Gérer les erreurs lors de la réception de documents électroniques
1. Dans la fenêtre **Documents entrants** , sélectionnez la ligne pour un document électronique en provenance du service OCR et contenant des erreurs. Elle est indiquée par la valeur Erreur dans le champ **Statut OCR**.
2. Sélectionnez l'option **Modifier** pour ouvrir la fenêtre **Document entrant**.
3. Sur le raccourci **Erreurs et avertissements**, sélectionnez le message, puis choisissez l'action **Ouvrir l'enregistrement associé**.
4. La fenêtre contenant les données erronées ou manquantes, comme une fiche fournisseur avec la valeur champ manquant, s'ouvre.
5. Corrigez l'erreur ou les erreurs en suivant les instructions de chaque message d'erreur.
6. Traitez maintenant le document électronique entrant en cliquant à nouveau sur le bouton **Créer manuellement**.
7. Répétez les étapes 5 et 6 pour toute erreur restante jusqu'à ce que le document électronique puisse être envoyé avec succès.

## <a name="to-train-the-ocr-service-to-avoid-errors"></a>Pour former le service OCR à éviter les erreurs
Comme le service OCR est basé sur la reconnaissance optique, il est probable qu'il interprète de manière incorrecte les caractères des fichiers PDF ou image lorsqu'il traite pour la première fois les documents d'un certain fournisseur, par exemple. Il peut ne pas interpréter le logo de la société comme le nom du fournisseur ou il peut mal interpréter le montant total sur un reçu de dépenses en raison de sa disposition. Pour éviter que ces erreurs se propagent, vous pouvez corriger les données reçues par le service OCR et envoyer les commentaires au service.

La fenêtre **Correction des données OCR**, que vous ouvrez à partir de la fenêtre **Document entrant**, affiche les champs du raccourci **Informations financières** dans deux colonnes, une avec les données OCR modifiables et une avec les données OCR en lecture seule. Lorsque vous sélectionnez le bouton **Envoyer des commentaires OCR**, le contenu de la fenêtre **Correction des données OCR** est envoyé au service OCR. La prochaine fois que le service traite les fichiers PDF ou image contenant les données en question, vos corrections seront intégrées pour éviter les mêmes erreurs.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Documents entrants**, puis sélectionnez le lien connexe.
2. Ouvrez un enregistrement de document entrant contenant les données reçues du service OCR, que vous souhaitez corriger.
3. Dans la fenêtre **Document entrant**, sélectionnez l'action **Corriger les données OCR**.
4. Dans la fenêtre, **Correction des données OCR**, remplacez les données de la colonne modifiable pour chaque champ dont la valeur est incorrecte.
5. Pour annuler les corrections effectuées depuis l'ouverture de la fenêtre **Correction des données OCR**, sélectionnez l'action **Réinitialiser les données OCR**.
6. Pour envoyer les corrections au service OCR, sélectionnez l'action **Envoyer des commentaires OCR**.
7. Pour enregistrer les corrections, fermez la fenêtre **Correction des données OCR**.

Les champs du raccourci **Informations financières** de la fenêtre **Document entrant** sont mis à jour avec les nouvelles valeurs que vous avez entrées à l'étape 4.

## <a name="see-also"></a>Voir aussi  
[Traiter les documents entrants](across-process-income-documents.md)  
[Documents entrants](across-income-documents.md)  
[Gestion des achats](purchasing-manage-purchasing.md)  
[Utiliser Dynamics NAV](ui-work-product.md)
