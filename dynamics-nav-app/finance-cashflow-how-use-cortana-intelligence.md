---
title: "Procédure : Effectuer des prévisions de trésorerie"
author: bholtorf
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 154fcaef89af0f6a131f4bcf0e9cf9a3f85f5903
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-make-predictive-cash-flow-forecasts"></a>Procédure : Effectuer des prévisions de trésorerie
Les prévisions de trésorerie vous permettent de garantir que votre société a suffisamment de trésorerie disponible pour répondre à ses obligations financières. En outre, elles sont utiles afin d'identifier les ajustements. Par exemple, si vous avez un surplus de trésorerie, vous pouvez rembourser certaines dettes ; vous apprécierez également un avertissement si vous arrivez à court de trésorerie. 

Cortana Intelligence utilise le service Azure Machine Learning pour effectuer des prévisions fiables. Par exemple, les prévisions issues de Cortana Intelligence peuvent vous aider à prévoir et à éviter les déficits de trésorerie. Le service combine les informations historiques avec les validations actuelles pour les recettes et les dépenses, notamment les validations des échéances à venir. Ces valeurs sont les suivantes :
* Commandes achat
* Commandes vente
* Factures achats et ventes validées
* Avoirs

## <a name="before-you-start"></a>Avant de commencer  
Avant d'utiliser Cortana Intelligence pour les prévisions de trésorerie, il convient de respecter certains points : 
* Si vous n'avez pas déjà utilisé les prévisions de trésorerie, vous devrez configurer :
    * une ou plusieurs configurations dans **Paramètres trésorerie** ; 
    * les comptes pour les clients et les fournisseurs, les commandes vente et les commandes achat. Cortana Intelligence utilise les validations dans ces comptes.
    * une ou plusieurs prévisions de trésorerie dans **Prévision de trésorerie**. Veillez à inclure les commandes achat, les commandes vente, les comptes fournisseurs et clients comme sources.  
    Pour en savoir plus, recherchez _prévisions de trésorerie_ dans le système d'aide. 
* Il convient de connaître l'URL d'API et la clé d'API pour le service Web prévisionnel à utiliser.  
    Vous pouvez utiliser Azure Machine Learning ou un autre service, si vous en avez un. Sinon, un modèle public désigné _Modèle de prévision pour Microsoft Dynamics NAV_ est disponible en ligne dans la galerie Cortana Intelligence. Pour utiliser le modèle, procédez comme suit :

    1. Dans un navigateur, accédez à la [Galerie Cortana Intelligence](https://go.microsoft.com/fwlink/?linkid=828352)
    2. Recherchez _Modèle prévisionnel pour Microsoft Dynamics NAV_, puis ouvrez-le dans Azure Machine Learning Studio.
    3. Utilisez votre compte Microsoft pour enregistrer un espace de travail, puis copiez le modèle.
    4. Exécutez le modèle, et publiez-le comme service Web.
    5. Notez l'URL d'API et la clé d'API. Vous utiliserez ces identifiants lors de la configuration de Cortana Intelligence dans Microsoft Dynamics NAV.  

* Réfléchissez à la fréquence du calcul des prévisions. Le service Azure Machine Learning a des limites en matière d'utilisation. Par exemple, si vous avez plusieurs articles, il peut s'avérer judicieux de faire des calculs moins fréquemment. 
* Soyez affecté au tableau de bord Comptable. 

## <a name="set-up-cortana-intelligence"></a>Configurer Cortana Intelligence
Vous pouvez utiliser un guide de configuration assistée pour configurer les prévisions de trésorerie. Le guide vous aide à spécifier des éléments, tels que la fréquence de mise à jour des prévisions, les comptes sur lesquels les baser, les informations concernant l'échéance de paiement des taxes et s'il convient d'utiliser Cortana Intelligence.  

Si vous utilisez déjà les prévisions de trésorerie et si vous souhaitez simplement activer Cortana Intelligence, vous pouvez également utiliser une procédure manuelle. Lors de votre connexion, une notification s'affiche dans une barre bleue en haut de l'espace de travail. Pour configurer immédiatement Cortana Intelligence, sélectionnez **Oui**. Le message s'affiche une seule fois. Si vous le fermez, utilisez la procédure manuelle pour configurer Cortana Intelligence.  

**Astuce :** tenez compte de la durée des périodes utilisée par le service lors de ses calculs. Plus vous fournissez de données, plus les prévisions seront précises. En outre, soyez prudent en ce qui concerne les grands écarts entre les périodes. Cela aura également un impact sur les prévisions. Si Cortana Intelligence ne trouve pas suffisamment de données ou si les données varient considérablement, le service ne fera pas de prévisions. 

Pour utiliser le guide de configuration assistée :
1. Dans le tableau de bord Comptable, sous le graphique **Prévisions de trésorerie**, sélectionnez l'action **Ouvrir la configuration assistée**.
2. Complétez les champs au besoin lors de chaque étape du guide.

Pour utiliser une procédure manuelle :
1. Recherchez **Paramètres trésorerie**, puis sélectionnez le lien associé.
2. Développez le raccourci **Cortana Intelligence**, puis complétez les champs, au besoin.

## <a name="turn-on-cortana-intelligence-for-cash-flow-forecasts"></a>Activez Cortana Intelligence pour les prévisions de trésorerie
1. Recherchez **Prévisions de trésorerie**, puis sélectionnez le lien associé.
2. Sélectionnez l'action **Feuille trésorerie**.
3. Sur la page **Feuille trésorerie**, sélectionnez l'action **Proposer lignes feuille activité**.  
4. Sous **Types origine à inclure**, cochez la case **Prévision Cortana Intelligence**.

## <a name="investigate-a-cash-flow-forecast"></a>Étudiez une prévision de trésorerie
Pour bien observer les données qui se cachent derrière les prévisions, notamment l'écart, sélectionnez la colonne **Cortana Intelligence**. La première ligne du tableau affiche l'écart. Les autres lignes sont organisées par document source.  

Par exemple, vous pouvez voir comment les prévisions :    
* gèrent les ventes et les achats confirmés ; 
* retirent les dépenses et ajoutent les recettes ;
* ignorent les commandes ventes et les commandes achats en double.

## <a name="see-also"></a>Voir aussi  
[Utiliser Dynamics NAV](ui-work-product.md)

