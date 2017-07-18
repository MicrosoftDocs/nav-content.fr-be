---
title: "Dépannage de l'inscription en self-service"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 931c427518694cbd0003ea82735292a019b388d5
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="troubleshooting-self-service-sign-up"></a>Dépannage de l'inscription en self-service
L'inscription à Dynamics NAV est simple et peut être effectuée très rapidement. Vous pouvez créer un compte gratuit même si vous représentez une société existante. Cet article aborde les problèmes que vous pouvez rencontrer lors de l'inscription.

## <a name="what-email-address-can-i-use-with-dynamics-nav"></a>Quelle adresse e-mail puis-je utiliser avec Dynamics NAV ?
Dynamics NAV exige que vous utilisiez une adresse e-mail professionnelle ou scolaire pour votre inscription. Dynamics NAV ne prend pas en charge les adresses e-mail fournies par les services de messagerie publics ni les opérateurs de télécommunications. Cela comprend outlook.com, hotmail.com, gmail.com, et d'autres.

Si vous essayez d'effectuer votre inscription à l'aide d'une adresse e-mail personnelle, vous recevez un message vous demandant d'utiliser une adresse professionnelle ou scolaire.

## <a name="troubleshooting"></a>Incident
Dans de nombreux cas, vous pouvez effectuer votre inscription à Dynamics NAV en suivant simplement le processus d'inscription. Toutefois, il existe plusieurs raisons pour lesquelles vous pouvez ne pas être en mesure de terminer l'inscription en self-service. La table ci-dessous récapitule certaines des raisons les plus courantes pour lesquelles vous pouvez ne pas être en mesure de terminer l'inscription en self-service, ainsi que des solutions pour remédier au problème.

|Symptôme/Message d'erreur                                                                             |Cause et solution de contournement|
|--------------------------------------------------------------------------------------------------|--------------------|
|Pour les adresses e-mail Office 365 qui ne sont pas enregistrés aux États-Unis, vous recevez un message semblable au suivant lors de votre inscription : <br>**L'inscription n'a pas fonctionné. Nous ne prenons pas encore en charge votre pays ou région.**<br> |À l'heure actuelle, Dynamics NAV prend uniquement en charge les comptes de messagerie Office 365 enregistrés aux États-Unis.|
|Les adresse e-mail personnelles telles que nancy@gmail.com ne sont pas prises en charge. Vous recevez un message semblable au suivant lors de votre inscription : <br>**Vous avez saisi une adresse e-mail personnelle. Veuillez saisir votre adresse e-mail professionnelle de sorte que nous puissions stocker les données de votre société en toute sécurité.**<br> Ou <br> **Il semble que votre adresse soit une adresse personnelle. Saisissez votre adresse professionnelle de sorte que vous puissions vous mettre en relation avec d'autres utilisateurs de votre société. Et vous ne inquiétez pas. Nous ne partagerons votre adresse avec personne.** | Dynamics NAV ne prend pas en charge les adresses e-mail fournies par les services de messagerie publics ni les opérateurs de télécommunications. Pour terminer l'inscription, essayez de nouveau en utilisant une adresse e-mail affectée par votre entreprise ou établissement scolaire. Si vous ne parvenez toujours pas à vous inscrire et que vous êtes disposé à effectuer un processus de configuration plus avancé, vous pouvez prendre un nouvel abonnement gratuit Office 365 et utiliser cette adresse e-mail pour vous inscrire.
|Adresses e-mail .gov ou .mil. Vous recevez un message semblable au suivant lors de votre inscription : <br>**Dynamics NAV n'est pas disponible : Dynamics NAV n'est pas disponible pour les utilisateurs ayant des adresses e-mail .gov ou .mil. pour le moment. Utilisez une autre adresse e-mail professionnelle ou vérifiez ultérieurement.** <br>Ou <br>**Nous ne sommes pas en mesure de terminer votre inscription. Il semble que Dynamics NAV ne soit pas disponible à l'heure actuelle pour votre entreprise ou établissement scolaire.**|À l'heure actuelle, Dynamics NAV ne prend pas en charge les adresses e-mail .gov ou .mil.|
|L'inscription en self-service n'est pas activée. Vous recevez un message semblable au suivant lors de votre inscription : <br>**Nous ne sommes pas en mesure de terminer votre inscription. Votre service informatique a désactivé l'inscription à Dynamics NAV. Pour terminer votre inscription, contactez votre service informatique.** <br>Ou <br> **Il semble que votre adresse soit une adresse personnelle. Saisissez votre adresse professionnelle de sorte que vous puissions vous mettre en relation avec d'autres utilisateurs de votre société. Et vous ne inquiétez pas. Nous ne partagerons votre adresse avec personne.**|L'administrateur informatique de votre entreprise a désactivé l'inscription en self-service à Dynamics NAV. Pour terminer votre inscription, contactez votre administrateur informatique et demandez-lui de suivre les instructions sur la page ci-dessous afin d'autoriser les utilisateurs existants à s'inscrire à Dynamics NAV et d'autoriser les nouveaux utilisateurs à rejoindre votre abonnement existant. Vous pouvez également rencontrer ce problème si vous avez effectué votre inscription à Office 365 par l'intermédiaire d'un partenaire.|
|L'adresse e-mail n'est pas un ID Office 365. Vous recevez un message semblable au suivant lors de votre inscription : <br>**Nous ne vous trouvons pas sur contoso.com. Utilisez-vous un autre identifiant dans votre entreprise ou établissement scolaire ? Essayez d'effectuer votre inscription avec celui-ci. Si cela ne fonctionne pas, contactez votre service informatique.**|Votre entreprise utilise pour l'inscription à Office 365 et à d'autres services Microsoft des identifiants différents de votre adresse e-mail. Par exemple, votre adresse e-mail peut être Nancy.Smith@contoso.com alors que votre identifiant est nancys@contoso.com. Pour terminer votre inscription, utilisez l'identifiant que votre entreprise vous a affecté pour l'inscription à Office 365 ou à d'autres services Microsoft. Si vous ne connaissez pas cet identifiant, contactez votre administrateur informatique. Si vous ne parvenez toujours pas à vous inscrire et que vous êtes en mesure d'effectuer un processus de configuration plus avancé, vous pouvez prendre un nouvel abonnement gratuit Office 365 et utiliser cette adresse e-mail pour vous inscrire.|


## <a name="see-also"></a>Voir aussi
[Bienvenue dans Dynamics NAV](across-get-started.md)  
[Utiliser Dynamics NAV](ui-work-product.md)




