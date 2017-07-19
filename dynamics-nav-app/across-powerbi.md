---
title: Utilisation du pack de contenu pour Power BI de Dynamics NAV
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6351e4819a2f3665cc561b5b1f868eea5d435f75
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="using-the-dynamics-nav-content-pack-for-power-bi"></a>Utilisation du pack de contenu pour Power BI de Dynamics NAV
Il est facile d'obtenir des informations exploitables de vos données Dynamics NAV grâce à Power BI et au pack de contenu Dynamics NAV. Power BI extrait vos données, puis génère un tableau de bord prêt à l'emploi et des états basés sur ces données.  

Le pack de contenu est pré-configuré pour fonctionner avec les données de vente et les données financières provenant de la société de démonstration que vous obtenez lorsque vous vous inscrivez à l'aperçu Dynamics NAV.  

- Sélectionnez un visuel du tableau de bord pour ouvrir l'un des états sept sous-jacents.  
- Filtrez l'état ou ajoutez les champs que vous souhaitez contrôler.  
- Épinglez cette vue personnalisée au tableau de bord pour continuer à effectuer le suivi.  
Le tableau de bord et les états sous-jacents sont actualisés au quotidien. Vous pouvez contrôler le programme de réactualisation et en modifier la fréquence sur l'ensemble de données.  

## <a name="accessing-dynamics-nav-in-power-bi"></a>Accéder à Dynamics NAV dans Power BI
Pour afficher vos données Dynamics NAV dans Power BI, vous devez disposer des éléments suivants :  

- Accès à Dynamics NAV. Pour en savoir plus, voir [Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=759714).  
- Accès à Power BI. Pour plus d'informations, reportez-vous à [Power BI](https://powerbi.microsoft.com).

Sur le site Power BI, vous trouverez des informations supplémentaires relatives à [l'ajout du pack de contenu Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=760850) à Power BI.  

Pour accéder au pack de contenu Dynamics NAV dans Power BI, dans la fenêtre de connexion, vous devez spécifier les informations suivantes :

| Champ       | Description              |
|-------------|--------------------------|
|**URL de flux OData**|L'URL OData permet à Power BI d'accéder aux données de votre société, par exemple https://monentreprise.com:7048/MS/OData/Société('CRONUS%20US').|
|**Méthode d'authentification**|Sélectionnez **Basique**.|
|**Nom utilisateur**|Le compte de messagerie que vous avez utilisé pour vous inscrire à Dynamics NAV, par exemple *me@mybusiness.com*.|
|**Mot de passe**|Il s'agit de la clé d'accès rapide au service Web pour votre compte d'utilisateur dans Dynamics NAV.|

Cela signifie que vous devez extraire deux informations de Dynamics NAV : l'URL OData et la clé d'accès rapide au service Web pour votre compte utilisateur.  
**Obtention de l'URL**  
Lorsque vous ajoutez Dynamics NAV à Power BI, vous devez spécifier une URL pour que Power BI puisse accéder aux données de votre société. Dans la fenêtre de connexion, l'URL est appelée **URL de flux OData** et doit avoir le format suivant :

         https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
Dans cet exemple, *monentreprise* est le nom de votre service Dynamics NAV, *CRONUS US* est le nom de la société de démonstration et *%20* représente l'espace dans le nom.   
Pour obtenir l'URL, dans Dynamics NAV, recherchez et ouvrez la fenêtre **Services web**. Cette fenêtre répertorie les services Web actuellement disponibles, et vous pouvez copier le lien du champ **URL OData** pour l'un des services Web OData par défaut.  
**Obtention de la clé d'accès au service web**  
Pour utiliser les données de Dynamics NAV, dans Power BI, dans la fenêtre **Connexion à Dynamics NAV**, vous devez indiquer votre nom d'utilisateur (votre compte de messagerie) et mots de passe. Le mot de passe correspond à la clé d'accès rapide au service Web définie pour votre compte utilisateur dans Dynamics NAV.  
Pour obtenir une clé d'accès rapide au service Web, dans Dynamics NAV, recherchez la fenêtre **Utilisateurs**, puis ouvrez la fiche de votre compte utilisateur. Sur le raccourci **Accès service web**, copiez le contenu du champ **Clé d'accès service web**. Si le champ est vierge, sélectionnez dans le ruban **Modifier la clé d'accès service web**, sélectionnez le champ **La clé n'expire jamais**, puis cliquez sur le bouton OK. Vous pouvez alors copier la clé.  

## <a name="getting-data-from-dynamics-nav"></a>Obtention de données de Dynamics NAV
Le tableau de bord Dynamics NAV affiche les états les plus courants que vous utiliserez pour effectuer le suivi de votre activité. Les données sont extraite de votre société Dynamics NAV en utilisant les services Web pour lire les données en temps réel. Dans Dynamics NAV, la fenêtre **Services Web** répertorie les services Web qui ont été configurés pour vous, y compris les suivants qui sont utilisés par le pack de contenu dans Power BI :  

- ItemSalesAndProfit  
- ItemSalesByCustomer  
- powerbifinance-setup  
- SalesDashboard  
- SalesOpportunities  
- SalesOrdersBySalesPerson  
- TopCustomerOverview  

**Remarque** : si vous modifiez le nom de l'un de ces services Web, les données ne s'affichent pas dans Power BI.  
Si vous souhaitez ajouter et utiliser d'autres données dans Power BI, vous devez trouver les tables dans Dynamics NAV, les exposer comme services Web, puis les ajouter au pack de contenu. Il s'agit d'un scénario avancé, et nous vous recommandons de commencer avec les données déjà disponibles dans Power BI.  

## <a name="troubleshooting"></a>Incident
Le tableau de bord Power BI s'appuie sur les services Web publiés qui sont répertoriés ci-dessus. Il affichera les données de la société de démonstration ou de votre propre société si vous importez les données de votre solution financière actuelle. Toutefois, si une erreur se produit, cette section fournit une solution de rechange pour les problèmes les plus courants.  

**« Échec de la validation des paramètres, assurez-vous que tous les paramètres sont valides »**  
Si ce message d'erreur s'affiche une fois que vous avez saisi votre URL Dynamics NAV, assurez-vous que les conditions suivantes sont remplies :  

- L'URL suit exactement ce motif :

    https://monentreprise.projectmadeira.com:7048/MS/OData/Société('CRONUS%20US')  
- Supprimez tout texte qui suit le nom de la société entre parenthèse  
- Assurez-vous qu'il n'y a pas de barre oblique à la fin de l'URL.  
- Assurez-vous que la connexion est sécurisée, ce qui est indiqué par l'URL qui commence par *https*.  


**« Échec de la connexion »**  
Si vous obtenez un message d'erreur de type « échec de la connexion » lorsque vous vous connectez au tableau de bord à l'aide de vos informations d'identification Dynamics NAV, cela peut être causé par l'un des problèmes suivants :

* Le compte que vous utilisez n'est pas doté des autorisations nécessaires pour lire les données Dynamics NAV de votre compte.

    Vérifiez votre compte utilisateur dans Dynamics NAV, vérifiez que vous avez utilisé la bonne clé d'accès rapide au service Web comme mot de passe, puis essayez de nouveau.  
* L'instance de Dynamics NAV à laquelle vous essayez de vous connecter n'est pas dotée d'un certificat SSL valide. Dans ce cas, vous obtiendrez un message d'erreur plus détaillé (« impossible d'établir une relation SSL fiable »).

    **Remarque** : les certificats auto-signés ne sont pas pris en charge.  


**« Oups »**  
Si une boîte de dialogue d'erreur « Oups » s'affiche une fois que vous avez passé la boîte de dialogue d'authentification, cela est généralement causé par un problème qui survient lors de la connexion aux données du pack de contenu.

* Vérifiez que l'URL suit le motif qui a été spécifié plus tôt :

    https://monentreprise.projectmadeira.com:7048/MS/OData/Société('CRONUS%20US')  
* Une erreur courante est de spécifier l'intégralité de l'URL pour un service Web spécifique :

    https://monentreprise.projectmadeira.com:7048/MS/OData/Société('CRONUS%20US')/powerbifinance-setup  
* Vous avez peut-être aussi oublié de spécifier le nom de la société :

    https://monentreprise.projectmadeira.com:7048/MS/OData/  


## <a name="see-also"></a>Voir aussi
[Bienvenue dans Dynamics NAV](across-get-started.md)  

