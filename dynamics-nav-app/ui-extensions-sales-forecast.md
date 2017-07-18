---
title: "Prévision de ventes et des stocks"
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 765527ed4f4800acec20f0abbd4374e95c9c36dc
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="sales-and-inventory-forecast-for-dynamics-nav"></a>Prévisions des ventes et des stocks pour Dynamics NAV
La gestion des stocks est un compromis entre le service client et la gestion de vos coûts. D'une part, un stock faible exige un capital travail inférieur, mais d'autre part, les ruptures de stock mènent potentiellement à des ventes non concrétisées. L'extension Sales and Inventory Forecast prévoit les ventes potentielles à l'aide des données historiques et donne une présentation claire des ruptures de stock prévues. Selon la prévision, l'extension aide à créer des demandes de réapprovisionnement auprès de vos fournisseurs et vous fait gagner du temps.  

## <a name="setting-up-forecasting"></a>Paramétrage des prévisions
Dans Dynamics NAV, vous devez configurer la connexion à Azure Machine Learning (Azure ML). Pour en savoir plus, voir [Procédure : Enregistrer une solution Dynamics NAV sur le portail Azure Management](ui-how-register-dynamics-nav-azure.md). Une fois la connexion établie, vous pouvez configurer les prévisions pour utiliser un autre type de période pour exécuter votre rapport, par exemple en passant des prévisions mensuelles aux prévisions trimestrielles. Vous pouvez également choisir le nombre de périodes à partir desquelles calculer les prévisions, selon le degré de granularité que vous souhaitez accorder à vos prévisions. Nous vous proposons de faire des prévisions mensuelles avec un horizon à 12 mois.  

## <a name="using-the-forecasts"></a>À l'aide des prévisions
Cette extension utilise les capacités d'apprentissage automatique de Microsoft Azure pour prévoir les ventes futures en fonction de votre historique des ventes pour vous aider à éviter les ruptures de stock. Par exemple, lorsque vous choisissez un article dans la fenêtre **Articles**, le graphique du volet **Prévision des articles** affiche les ventes estimées de cet article dans la période à venir. Ainsi vous pouvez voir si vous risquez d'être bientôt en rupture de stock pour l'article.  

Vous pouvez également utiliser l'extension pour suggérer quand réapprovisionner les stocks. Par exemple, si vous créez un bon de commande pour Fabrikam, car vous souhaitez acheter leur nouvelle chaise de bureau, l'extension Sales and Inventory Forecast vous suggèrera également de réapprovisionner la chaise dactylo LONDON que vous achetez généralement auprès de ce fournisseur. En effet, les prévisions de l'extension indiquent que vous allez arriver en rupture de stocks concernant la chaise dactylo LONDON dans les deux prochaines semaines. Aussi, nous vous recommandons de commander davantage de chaises dès à présent.  

## <a name="see-also"></a>Voir aussi
[Gestion des ventes](sales-manage-sales.md)  
[Gestion du stock](inventory-manage-inventory.md)  
[Personnalisation de Dynamics NAV à l'aide des extensions](ui-extensions.md)  
[Procédure : Enregistrer Dynamics NAV sur le portail Azure Management](ui-how-register-dynamics-nav-azure.md)  

