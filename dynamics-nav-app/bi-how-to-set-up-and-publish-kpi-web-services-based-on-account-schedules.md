---
title: "Procédure de configuration et de publication des services Web KPI sur la base de tableaux d'analyse"
description: "La fenêtre **Tableau d'analyse - Paramètres du service web KPI** vous permet de configurer la manière dont les informations KPI du tableau d'analyse sont affichées et sur quels tableaux d'analyse spécifiques baser les KPI."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b45fe6e1e5d4e5be00a6e8a34b7b4fea39b5d75b
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-and-publish-kpi-web-services-based-on-account-schedules"></a>Procédure de configuration et de publication des services Web KPI sur la base de tableaux d'analyse
La fenêtre **Tableau d'analyse - Paramètres du service web KPI** vous permet de configurer la manière dont les informations KPI du tableau d'analyse sont affichées et sur quels tableaux d'analyse spécifiques baser les KPI. Lorsque vous sélectionnez le bouton **Publier le service Web**, les informations KPI du tableau d'analyse spécifiées sont ajoutées à la liste des services Web publiés dans la fenêtre **Services web**.  

## <a name="to-set-up-and-publish-a-kpi-web-service-that-is-based-on-account-schedules"></a>Configuration et de publication d'un service Web KPI sur la base de tableaux d'analyse  

1.  Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Tableau d'analyse - Paramètres du service web KPI**, puis choisissez le lien associé.  
2.  Sous le raccourci **Général**, renseignez les champs comme indiqué dans le tableau ci-dessous.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Début valeurs prévues**|Spécifiez la date à laquelle les valeurs prévues sont affichées sur le graphique KPI du tableau d'analyse.<br /><br /> Les valeurs prévues sont récupérées à partir du budget en comptabilité que vous sélectionnez dans le champ **Nom budget comptable**. **Note ::** pour obtenir des KPI qui affichent les chiffres prévus après une certaine date et les chiffres réels avant cette date, vous pouvez modifier le champ **Début période validation** dans la fenêtre **Paramètres comptabilité**. Pour plus d'informations, voir Début période validation.|  
    |**Nom budget comptable**|Spécifiez le nom du budget en comptabilité qui fournit les valeurs prévues au service Web KPI du tableau d'analyse.|  
    |**Période**|Indiquez la période sur laquelle le service Web KPI du tableau d'analyse se base.|  
    |**Afficher par**|Indiquez l'intervalle de temps dans lequel le KPI du tableau d'analyse est affiché.|  
    |**Nom du service web**|Indiquez le nom du service Web KPI du tableau d'analyse.<br /><br /> Ce nom est affiché dans le champ **Nom de service** dans la fenêtre **Services web**.|  

    Procédez à la spécification d'un ou plusieurs tableaux d'analyse que vous souhaitez publier en tant que service Web KPI en fonction du paramétrage que vous avez fait dans la table précédente.  

3.  Sous le raccourci **Tableaux d'analyse**, renseignez les champs comme indiqué dans le tableau ci-dessous.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom tableau d'analyse**|Permet d'indiquer le tableau d'analyse sur lequel le service Web KPI se base.|  
    |**Description tableau analyse**|Permet d'indiquer la désignation du tableau d'analyse sur lequel le service Web KPI se base.|  

4.  Répétez l'étape 3 pour tous les tableaux d'analyse sur lesquels vous souhaitez baser le service Web KPI du tableau d'analyse.  
5.  Pour visualiser ou modifier le tableau d'analyse sélectionné, sur le raccourci **Tableau d'analyse**, choisissez l'action **Modifier tableau d'analyse**.  
6.  Pour afficher les informations KPI du tableau d'analyse que vous avez définies, choisissez l'action **Tableau d'analyse - Paramètres du service web KPI**.  
7.  Pour publier le service Web KPI du tableau d'analyse, choisissez l'action **Publier le service web**. Le service Web est ajouté à la liste des services Web publiés dans la fenêtre **Web Services**.  

    > [!NOTE]  
    >  V-us pouvez également publier le service Web KPI en pointant vers l'objet de page **Tableau d'analyse\-Paramètres du service web KPI** à partir de la fenêtre**Services web**. Pour plus d'informations, voir [Procédure : publication d'un service web](https://msdn.microsoft.com/en-us/library/dd338978.aspx) sur MSDN.  

## <a name="see-also"></a>Voir aussi  
[Veille économique](bi.md)  
[Finances](finance.md)  
[Configuration de Finance](finance-setup-finance.md)  
[Les écritures comptables et le plan comptable](finance-general-ledger.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

