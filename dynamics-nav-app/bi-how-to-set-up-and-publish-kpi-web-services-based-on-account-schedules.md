---
title: "Procédure de configuration et de publication des services Web KPI sur la base de tableaux d'analyse"
description: "La fenêtre **Tableau d'analyse - Paramètres du service web KPI** vous permet de configurer la manière dont les informations KPI du tableau d'analyse sont affichées et sur quels tableaux d'analyse spécifiques baser les KPI."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
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
# <a name="how-to-set-up-and-publish-kpi-web-services-based-on-account-schedules"></a><span data-ttu-id="e7f8d-103">Procédure de configuration et de publication des services Web KPI sur la base de tableaux d'analyse</span><span class="sxs-lookup"><span data-stu-id="e7f8d-103">How to: Set Up and Publish KPI Web Services Based on Account Schedules</span></span>
<span data-ttu-id="e7f8d-104">La fenêtre **Tableau d'analyse - Paramètres du service web KPI** vous permet de configurer la manière dont les informations KPI du tableau d'analyse sont affichées et sur quels tableaux d'analyse spécifiques baser les KPI.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-104">In the **Account Schedule KPI Web Service Setup** window, you set up how to show the account-schedule KPI data and which specific account schedules to base the KPIs on.</span></span> <span data-ttu-id="e7f8d-105">Lorsque vous sélectionnez le bouton **Publier le service Web**, les informations KPI du tableau d'analyse spécifiées sont ajoutées à la liste des services Web publiés dans la fenêtre **Services web**.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-105">When you choose the **Publish Web Service** button, the specified account-schedule KPI data is added to the list of published web services in the **Web Services** window.</span></span>  

## <a name="to-set-up-and-publish-a-kpi-web-service-that-is-based-on-account-schedules"></a><span data-ttu-id="e7f8d-106">Configuration et de publication d'un service Web KPI sur la base de tableaux d'analyse</span><span class="sxs-lookup"><span data-stu-id="e7f8d-106">To set up and publish a KPI web service that is based on account schedules</span></span>  

1.  <span data-ttu-id="e7f8d-107">Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Tableau d'analyse - Paramètres du service web KPI**, puis choisissez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedule KPI Web Service Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e7f8d-108">Sous le raccourci **Général**, renseignez les champs comme indiqué dans le tableau ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-108">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="e7f8d-109">Champ</span><span class="sxs-lookup"><span data-stu-id="e7f8d-109">Field</span></span>|<span data-ttu-id="e7f8d-110">Désignation</span><span class="sxs-lookup"><span data-stu-id="e7f8d-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="e7f8d-111">**Début valeurs prévues**</span><span class="sxs-lookup"><span data-stu-id="e7f8d-111">**Forecasted Values Start**</span></span>|<span data-ttu-id="e7f8d-112">Spécifiez la date à laquelle les valeurs prévues sont affichées sur le graphique KPI du tableau d'analyse.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-112">Specify at what point in time forecasted values are shown on the account-schedule KPI graphic.</span></span><br /><br /> <span data-ttu-id="e7f8d-113">Les valeurs prévues sont récupérées à partir du budget en comptabilité que vous sélectionnez dans le champ **Nom budget comptable**.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-113">The forecasted values are retrieved from the general ledger budget that you select in the **G/L Budget Name** field.</span></span> <span data-ttu-id="e7f8d-114">**Note ::** pour obtenir des KPI qui affichent les chiffres prévus après une certaine date et les chiffres réels avant cette date, vous pouvez modifier le champ **Début période validation** dans la fenêtre **Paramètres comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-114">**Note:**  To obtain KPIs that show forecasted figures after a certain date and actual figures before the date, you can change the **Allow Posting From** field in the **General Ledger Setup** window.</span></span> <span data-ttu-id="e7f8d-115">Pour plus d'informations, voir Début période validation.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-115">For more information, see Allow Posting From.</span></span>|  
    |<span data-ttu-id="e7f8d-116">**Nom budget comptable**</span><span class="sxs-lookup"><span data-stu-id="e7f8d-116">**G/L Budget Name**</span></span>|<span data-ttu-id="e7f8d-117">Spécifiez le nom du budget en comptabilité qui fournit les valeurs prévues au service Web KPI du tableau d'analyse.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-117">Specify the name of the general ledger budget that provides forecasted values to the account-schedule KPI web service.</span></span>|  
    |<span data-ttu-id="e7f8d-118">**Période**</span><span class="sxs-lookup"><span data-stu-id="e7f8d-118">**Period**</span></span>|<span data-ttu-id="e7f8d-119">Indiquez la période sur laquelle le service Web KPI du tableau d'analyse se base.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-119">Specify the period that the account-schedule KPI web service is based on.</span></span>|  
    |<span data-ttu-id="e7f8d-120">**Afficher par**</span><span class="sxs-lookup"><span data-stu-id="e7f8d-120">**View By**</span></span>|<span data-ttu-id="e7f8d-121">Indiquez l'intervalle de temps dans lequel le KPI du tableau d'analyse est affiché.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-121">Specify which time interval the account-schedule KPI is shown in.</span></span>|  
    |<span data-ttu-id="e7f8d-122">**Nom du service web**</span><span class="sxs-lookup"><span data-stu-id="e7f8d-122">**Web Service Name**</span></span>|<span data-ttu-id="e7f8d-123">Indiquez le nom du service Web KPI du tableau d'analyse.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-123">Specify the name of the account-schedule KPI web service.</span></span><br /><br /> <span data-ttu-id="e7f8d-124">Ce nom est affiché dans le champ **Nom de service** dans la fenêtre **Services web**.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-124">This name will appear in the **Service Name** field in the **Web Services** window.</span></span>|  

    <span data-ttu-id="e7f8d-125">Procédez à la spécification d'un ou plusieurs tableaux d'analyse que vous souhaitez publier en tant que service Web KPI en fonction du paramétrage que vous avez fait dans la table précédente.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-125">Proceed to specify one or more account schedules that you want to publish as a KPI web service according to the setup that you made in the previous table.</span></span>  

3.  <span data-ttu-id="e7f8d-126">Sous le raccourci **Tableaux d'analyse**, renseignez les champs comme indiqué dans le tableau ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-126">On the **Account Schedules** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="e7f8d-127">Champ</span><span class="sxs-lookup"><span data-stu-id="e7f8d-127">Field</span></span>|<span data-ttu-id="e7f8d-128">Désignation</span><span class="sxs-lookup"><span data-stu-id="e7f8d-128">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="e7f8d-129">**Nom tableau d'analyse**</span><span class="sxs-lookup"><span data-stu-id="e7f8d-129">**Acc. Schedule Name**</span></span>|<span data-ttu-id="e7f8d-130">Permet d'indiquer le tableau d'analyse sur lequel le service Web KPI se base.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-130">Specify the account schedule that the KPI web service is based on.</span></span>|  
    |<span data-ttu-id="e7f8d-131">**Description tableau analyse**</span><span class="sxs-lookup"><span data-stu-id="e7f8d-131">**Acc. Schedule Description**</span></span>|<span data-ttu-id="e7f8d-132">Permet d'indiquer la désignation du tableau d'analyse sur lequel le service Web KPI se base.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-132">Specify the description of the account schedule that the KPI web service is based on.</span></span>|  

4.  <span data-ttu-id="e7f8d-133">Répétez l'étape 3 pour tous les tableaux d'analyse sur lesquels vous souhaitez baser le service Web KPI du tableau d'analyse.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-133">Repeat step 3 for all the account schedules that you want to base the account-schedule KPI web service on.</span></span>  
5.  <span data-ttu-id="e7f8d-134">Pour visualiser ou modifier le tableau d'analyse sélectionné, sur le raccourci **Tableau d'analyse**, choisissez l'action **Modifier tableau d'analyse**.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-134">To view or edit the selected account schedule, on the **Account Schedule** FastTab, choose the **Edit Account Schedule** action.</span></span>  
6.  <span data-ttu-id="e7f8d-135">Pour afficher les informations KPI du tableau d'analyse que vous avez définies, choisissez l'action **Tableau d'analyse - Paramètres du service web KPI**.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-135">To view the account-schedule KPI data that you have set up, choose the **Account Schedule KPI Web Service** action.</span></span>  
7.  <span data-ttu-id="e7f8d-136">Pour publier le service Web KPI du tableau d'analyse, choisissez l'action **Publier le service web**.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-136">To publish the account-schedule KPI web service, choose the **Publish Web Service** action.</span></span> <span data-ttu-id="e7f8d-137">Le service Web est ajouté à la liste des services Web publiés dans la fenêtre **Web Services**.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-137">The web service is added to the list of published web services in the **Web Services** window.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="e7f8d-138">V-us pouvez également publier le service Web KPI en pointant vers l'objet de page **Tableau d'analyse\-Paramètres du service web KPI** à partir de la fenêtre**Services web**.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-138">You can also publish the KPI web service by pointing to the **Account Schedule KPI Web Service Setup** page object from the **Web Services** window.</span></span> <span data-ttu-id="e7f8d-139">Pour plus d'informations, voir [Procédure : publication d'un service web](https://msdn.microsoft.com/en-us/library/dd338978.aspx) sur MSDN.</span><span class="sxs-lookup"><span data-stu-id="e7f8d-139">For more information, see [How to: Publish a Web Service](https://msdn.microsoft.com/en-us/library/dd338978.aspx) on MSDN.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e7f8d-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e7f8d-140">See Also</span></span>  
[<span data-ttu-id="e7f8d-141">Veille économique</span><span class="sxs-lookup"><span data-stu-id="e7f8d-141">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="e7f8d-142">Finances</span><span class="sxs-lookup"><span data-stu-id="e7f8d-142">Finance</span></span>](finance.md)  
[<span data-ttu-id="e7f8d-143">Configuration de Finance</span><span class="sxs-lookup"><span data-stu-id="e7f8d-143">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="e7f8d-144">Les écritures comptables et le plan comptable</span><span class="sxs-lookup"><span data-stu-id="e7f8d-144">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="e7f8d-145">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e7f8d-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
