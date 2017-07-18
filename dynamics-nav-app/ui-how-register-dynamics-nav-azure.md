---
title: "Procédure : Enregistrer Dynamics NAV sur le portail Azure Management"
author: edupont04
manager: edupont
ms.author: edupont
ms.custom: na
ms.date: 11/15/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 225773f7f686dd6e9a79f759d520d66f7e7b9d0a
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---
# <a name="how-to-register-dynamics-nav-in-the-azure-management-portal"></a>Procédure : Enregistrer Dynamics NAV sur le portail Azure Management
Si vous souhaitez utiliser les services basés sur Microsoft Azure, vous devez enregistrer votre solution Dynamics NAV sur le portail Azure Management. Par exemple, l'extension [Prévision des ventes et des stocks](ui-extensions-sales-forecast.md) exige que vous spécifiez une clé API et une URI de l'API. En outre, d'autres services nécessitent des informations similaires. Ainsi, où trouvez-vous ces informations ?

Vous pouvez utiliser le guide **Configurer le portail Azure Management** pour enregistrer votre solution Dynamics NAV sur le portail Azure Management et extraire les informations dont vous avez besoin pour utiliser les services, tels que l'extension Prévision des ventes et des stocks, Power BI, Office 365, etc. Vous devez vous enregistrer une seule fois sur le portail Azure Management, puis avoir les droits d'administrateur ou de super-utilisateur de la solution Dynamics NAV.

Concernant l'enregistrement, il est essentiel que Dynamics NAV et que le service auquel vous souhaitez vous connecter connaissent les informations Azure Active Directory (Azure AD) de chacun.

## <a name="to-register-dynamics-nav-in-the-azure-management-portal"></a>Pour enregistrer votre solution Dynamics NAV sur le portail Azure Management
1. Connectez-vous au portail Azure Management à l'adresse [https://portal.azure.com](https://portal.azure.com).
    Si vous débutez avec le portail Azure Management, vous trouverez une aide précieuse dans la [Bibliothèque de documents Azure](https://azure.microsoft.com/en-us/documentation/articles).
2. Dans le volet gauche de navigation, sélectionnez **Autres services**, puis **Enregistrements des applications**.
3. Dans le menu tout en haut de l'écran, sélectionnez **Ajouter**, puis dans **Créer un volet**, complétez les champs avec les informations suivantes :
    - **Nom** : spécifiez un nom pour votre solution Dynamics NAV, tel que *Dynamics NAV*.
    - **Type d'application** : sélectionnez **Application Web* / API**.
    - **URL de connexion** : saisissez l'URL pour votre client navigateur Dynamics NAV, tel que *https://MyServer:8080/DynamicsNAV/WebClient/OAuthLanding.htm*.
        Le fichier OAuthLanding.htm est un fichier qui aide à gérer l'échange de données entre Dynamics NAV et d'autres services via Azure AD.
4. Cliquez sur le bouton **Créer**.
    Cela ajoute votre solution Dynamics NAV au **volet Enregistrements d'applications**, afin que vous puissiez y ajouter des paramètres.
5. Dans la **liste Enregistrements d'applications**, sélectionnez votre nouvelle application. Si le volet **Paramètres** ne s'ouvre pas, vous devriez voir une action pour ouvrir le volet **Paramètres**.
6. Dans le volet **Paramètres**, dans la section **Accès API**, sélectionnez **Clés**.
7. Dans le volet **Clés**, spécifiez une description et la date d'expiration de la clé, puis sélectionnez **Enregistrer**.
8. Copiez la clé générée dans un emplacement temporaire. Vous en aurez besoin lors de la procédure suivante.
9. Dans la section **Accès API**, choisissez **Autorisations requises**.
    - Ajouter des autorisations déléguées pour afficher tous les états du service Power BI
    - Ajouter des autorisations déléguées pour valider et lire un profil utilisateur dans Windows Azure Active Directory
    - Répétez cette procédure pour les autres services auxquels vous souhaitez accorder l'accès à votre Dynamics NAV
10. Fermez le volet **Paramètres**, puis, dans le volet **Essentiels**, copiez la valeur de l'**ID d'application** vers un emplacement temporaire.

Vous avez désormais enregistré votre solution Dynamics NAV sur le portail Azure Management, vous avez donné l'accès aux services appropriés et vous avez extrait les informations dont vous avez besoin dans Dynamics NAV.  

## <a name="to-add-the-information-to-dynamics-nav"></a>Pour ajouter des informations dans Dynamics NAV
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Assistant Paramètres application Azure AD**, puis sélectionnez le lien connexe.
2. Dans l'assistant, sélectionnez **Suivant**.
3. Dans le champ **ID Client**, spécifiez le contenu que vous avez copié précédemment à partir du champ **ID d'application**.
4. Dans le champ **Clé secrète**, spécifiez le contenu que vous avez copié précédemment à partir du volet **Clés**.
5. Choisissez **Suivant**. Sauf si un message d'erreur s'affiche, vous avez terminé.

Votre solution Dynamics NAV est enregistrée et prête pour se connecter aux services tels que Cortana Intelligence et Power BI.

## <a name="see-also"></a>Voir aussi
[Prévision de ventes et des stocks](ui-extensions-sales-forecast.md)  
[Configurer votre solution Dynamics NAV](setup.md)  

