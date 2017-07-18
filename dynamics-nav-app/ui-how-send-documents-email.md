---
title: "Procédure : envoyer des documents par e-mail"
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: e4476c2ab903001017dcd6c8bdaa84892ba79c9e
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-send-documents-by-email"></a>Procédure : envoyer des documents par e-mail
Pour communiquer le contenu des documents commerciaux rapidement à vos partenaires commerciaux, par exemple les informations paiement sur les documents vente aux clients, vous pouvez utiliser la fonctionnalité de présentation des états pour définir le contenu spécifique aux documents qui est automatiquement inséré au corps du message.

Pour activer les e-mails au sein de Dynamics NAV, démarrez la configuration assistée **Configurer la messagerie** sur la page d'accueil.

Vous pouvez envoyer en pièce jointe à des e-mails virtuellement tous les types de documents directement à partir de la fenêtre qui affiche le document. Outre la pièce jointe, vous pouvez configurer des corps de message spécifique à des documents, avec des informations de base du document précédées d'un texte standard de salutations au destinataire du message et de présentation du document en question. Pour proposer à vos clients de payer les ventes par voie électronique à l'aide d'un service de paiement, comme Paypal par exemple, vous pouvez insérer les informations et le lien hypertexte Paypal dans le corps du message.

À partir de tous les documents pris en charge, vous initiez l'envoi d'e-mails en sélectionnant l'action **Envoyer** sur les documents validés, ou l'action **Valider et envoyer** sur les documents non validés.

Si le champ **E-mail** de la fenêtre **Envoyer le document à** est défini sur **Oui (Afficher une invite pour le réglage des paramètres)**, la fenêtre **Envoyer e-mail** s'affiche. Le champ **À :** est prérempli avec le contact et le document est en pièce jointe sous forme de fichier PDF. Dans le champ **Corps**, vous pouvez saisir un texte manuellement ou faire en sorte que le champ contienne un corps de message spécifique au document que vous avez configuré.

La procédure suivante décrit comment définir l'état **Ventes : Facture** à utiliser pour les corps de message spécifiques à un document lorsque vous envoyez par e-mail des factures vente validées.

## <a name="to-set-up-a-document-specific-email-body-for-sales-invoices"></a>Pour configurer corps de message spécifique à un document pour les factures vente
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Sélection des états - Ventes**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Sélection des états : Ventes**, dans le champ **Utilisation**, sélectionnez **Facture**
3. Sur une nouvelle ligne, dans le champ **ID état**, sélectionnez, par exemple, l'état standard 1306.
4. Cochez la case **Utiliser pour le corps du message e-mail**.
5. Sélectionnez le champ **ID présentation du corps du message e-mail**, puis sélectionnez l'une des présentations disponibles dans la fenêtre **Présentations état personnalisées**.
6. Les présentations d'état définissent à la fois le style et le contenu du corps de message, y compris le texte standard qui précède les informations de base relatives au document dans le corps du message.
7. Pour afficher ou modifier la présentation sur laquelle le corps du message est basé, dans la fenêtre **Présentations état personnalisées**, cliquez sur **Modifier présentation**.
8. Si vous souhaitez proposer à vos clients de payer les ventes par voie électronique, vous pouvez configurer le service de paiement associé, comme Paypal par exemple, puis insérer également les informations et le lien hypertexte Paypal dans le corps du message. Pour plus d'informations, reportez-vous à [Procédure : activer les paiements client via Paypal](sales-how-enable-customer-payments-paypal.md).
9. Cliquez sur le bouton **OK**.

Désormais, lorsque vous sélectionnez, par exemple, l'action Envoyer dans la fenêtre **Facture vente enregistrée**, le corps du message comporte les informations de document de l'état 1306 précédé d'un texte standard auquel sont appliqués des attributs de style en fonction de la présentation d'état que vous avez sélectionnée à l'étape 5.

La procédure suivante décrit comment envoyer une facture vente validée en tant que message e-mail avec le document en pièce jointe sous forme de fichier PDF et avec un corps de message spécifique au document.
## <a name="to-send-documents-by-email"></a>Pour envoyer des documents par e-mail
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Factures vente enregistrées**, puis sélectionnez le lien connexe.
2. Sélectionnez la facture vente appropriée, cliquez sur **Envoyer**. La fenêtre **Envoyer le document à** s'affiche.
3. Dans le champ **E-mail**, sélectionnez **Oui (Afficher une invite pour le réglage des paramètres)**. Pour plus d'informations, reportez vous à [Procédure : configurer des profils d'envoi de documents](sales-how-setup-document-send-profiles.md).
4. Cliquez sur le bouton **OK**. La fenêtre **Envoyer e-mail** s'affiche.
5. Dans le champ **À :**, entrez une adresse e-mail valide. La valeur par défaut est l'adresse e-mail du client.
6. Dans le champ **Cc**, spécifiez une adresse e-mail pour envoyer une copie du message à un autre destinataire.
7. Dans le champ **Cci**, spécifiez une adresse e-mail pour envoyer une copie de l'e-mail à un autre destinataire sans que cette adresse e-mail ni le nom n'apparaissent aux autres destinataires.
8. Dans le champ **Objet**, saisissez un texte descriptif de l'objet. La valeur par défaut est le nom du client et le numéro de facture.
9. Dans le champ **Document joint**, la facture générée est jointe par défaut en tant que fichier PDF. Cliquez sur le bouton de consultation pour ouvrir le fichier ou pour en joindre un autre.
10. Dans le champ **Corps**, entrez un message court au destinataire.

    Si le corps d'un message spécifique à un document est configuré dans la fenêtre **Sélection des états : Ventes**, le champ **Corps** est renseigné automatiquement. Pour plus d'informations, reportez-vous à la section « Pour configurer corps de message spécifique à un document pour les factures vente » de cette rubrique.
11. Cochez la case **Modifier dans Outlook Web App** pour ouvrir l'e-mail dans l'application de messagerie d'Office 365
12. Cliquez sur le bouton **OK** pour envoyer l'e-mail.

**Remarque** : si vous n'avez pas besoin de spécifier les paramètres d'e-mail à chaque fois que vous envoyez un document par e-mail, vous pouvez sélectionner l'option **Oui (Afficher une invite pour le réglage des paramètres)** dans le champ E-mail de la fenêtre **Envoyer le document à**. Dans ce cas, la fenêtre **Envoyer e-mail** ne s'affiche pas. Reportez-vous à l'étape 4. Pour plus d'informations, reportez vous à [Procédure : configurer des profils d'envoi de documents](sales-how-setup-document-send-profiles.md).

## <a name="see-also"></a>Voir aussi  
[Utiliser Dynamics NAV](ui-work-product.md)  
[Procédure : facturer des ventes](sales-how-invoice-sales.md)

