---
title: "Procédure : Facturer des projets"
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c0dcce83dfba30af38f33a6bf814b15862d5fc19
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-invoice-jobs"></a><span data-ttu-id="ff6a8-102">Procédure : Facturer des projets</span><span class="sxs-lookup"><span data-stu-id="ff6a8-102">How to: Invoice Jobs</span></span>
<span data-ttu-id="ff6a8-103">Au cours du projet, les coûts provenant de l'utilisation de ressources, de matières, et d'achats associés au projet peuvent s'accumuler.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-103">During the project, job costs from resource usage, materials, and job-related purchases can accumulate.</span></span> <span data-ttu-id="ff6a8-104">Au fur et à mesure de la progression du projet, ces transactions sont validées dans la feuille projet.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-104">As the job progresses, these transactions get posted to the job journal.</span></span> <span data-ttu-id="ff6a8-105">Il est important que tous les coûts enregistrés dans la feuille projet avant de facturer le client.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-105">It is important that all costs get recorded in the job journal before you invoice the customer.</span></span>

<span data-ttu-id="ff6a8-106">Vous pouvez facturer l'ensemble du projet à partir de la fenêtre **Lignes tâche projet** ou facturer uniquement les lignes facturables sélectionnées dans la fenêtre **Lignes planning**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-106">You can invoice the whole job from the **Job Task Lines** window or only invoice selected billable lines from the **Planning Lines** window.</span></span> <span data-ttu-id="ff6a8-107">La facturation peut avoir lieu une fois le projet terminé ou à certains intervalles au cours du projet sur la base d'une prévision de facture.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-107">Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.</span></span>

<span data-ttu-id="ff6a8-108">**Remarque** : Si vous sélectionnez **Facturable** dans le champ **Type ligne projet** dans les documents d'achat pour les achats associés au projet, les lignes planning projet prêtes pour facturation sont créées.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-108">**Note**: If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="ff6a8-109">Pour en savoir plus, reportez-vous à [Procédure : Gérer des fournitures d'un projet](projects-how-manage-project-supplies.md).</span><span class="sxs-lookup"><span data-stu-id="ff6a8-109">For more information, see [How to: Manage Project Supplies](projects-how-manage-project-supplies.md).</span></span>

## <a name="to-create-and-post-a-job-sales-invoice"></a><span data-ttu-id="ff6a8-110">Pour créer et valider une facture vente projet</span><span class="sxs-lookup"><span data-stu-id="ff6a8-110">To create and post a job sales invoice</span></span>  
<span data-ttu-id="ff6a8-111">Vous pouvez créer une facture pour un projet ou pour une ou plusieurs tâches projet pour un client lorsque le travail à facturer est terminé ou lorsque la date de facturation dépendante d'une prévision de facture est atteinte.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-111">You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.</span></span>

<span data-ttu-id="ff6a8-112">Dans la fenêtre **Projets**, vous pouvez facturer un client en sélectionnant le projet, puis en cliquant sur **Créer une facture vente projet**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-112">From the **Jobs** window, you can invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action.</span></span> <span data-ttu-id="ff6a8-113">La procédure suivante explique comment utiliser un traitement par lots pour facturer plusieurs projets.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-113">The following procedure shows how to use a batch job to invoice multiple jobs.</span></span>  

1. <span data-ttu-id="ff6a8-114">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projet Créer facture vente**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-114">In the top right corner, choose the **Search for Page or Report** icon, enter **Job Create Sales Invoice**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ff6a8-115">Renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-115">Fill in the fields as necessary.</span></span> <span data-ttu-id="ff6a8-116">Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-116">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="ff6a8-117">Définissez des filtres si vous souhaitez limiter le nombre de projets que le traitement par lots va traiter.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-117">Set filters if you want to limit the jobs that the batch job will process.</span></span>
3. <span data-ttu-id="ff6a8-118">Pour créer les factures, cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-118">Choose the **OK** button to create the invoices.</span></span>  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a><span data-ttu-id="ff6a8-119">Pour créer plusieurs factures vente projet à partir de lignes planning projet</span><span class="sxs-lookup"><span data-stu-id="ff6a8-119">To create multiple job sales invoices from job planning lines</span></span>  
<span data-ttu-id="ff6a8-120">Vous pouvez créer une facture à partir des lignes planning projet et indiquer à ce moment-là la quantité de l'article, la ressource ou le compte général sur lequel vous souhaitez facturer.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-120">You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.</span></span>

1. <span data-ttu-id="ff6a8-121">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projets**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-121">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="ff6a8-122">Ouvrez le projet approprié.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-122">Open a relevant job.</span></span>
3. <span data-ttu-id="ff6a8-123">Sélectionnez une tâche projet pour laquelle le champ **Type tâche projet** contient **Validation** puis, cliquez sur **Lignes planning projet**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-123">Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.</span></span>  
4. <span data-ttu-id="ff6a8-124">Dans une ligne planning projet, dans le champ **Qté à transférer à facturer**, saisissez la quantité de l'article, la ressource, le type de compte général sur lequel vous souhaitez facturer.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-124">On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.</span></span>  
5. <span data-ttu-id="ff6a8-125">Cliquez sur **Créer facture vente**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-125">Choose the **Create Sales Invoice** action.</span></span>
6. <span data-ttu-id="ff6a8-126">Dans la fenêtre **Projet Créer facture vente**, saisissez la date de validation et si vous souhaitez créer une facture ou ajouter cette facture à une facture existante.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-126">In the **Job Create Sales Invoice** window, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.</span></span>
7. <span data-ttu-id="ff6a8-127">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-127">Choose the **OK** button.</span></span>

    <span data-ttu-id="ff6a8-128">Dans la ligne planning projet, dans le champ **Qté à transférer à facturer**, vous pouvez visualiser la quantité.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-128">On the job planning line, in the **Qty. Transferred to Invoice** field, you can see the quantity.</span></span>

8. <span data-ttu-id="ff6a8-129">Dans la fenêtre **Lignes planning projet**, cliquez sur **Avoirs/Factures vente**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-129">In the **Job Planning Lines** window, choose the **Sales Invoices/Credit Memos** action.</span></span>

    <span data-ttu-id="ff6a8-130">La fenêtre **Facture vente** s'ouvre et affiche la quantité que vous avez transférée à la facture.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-130">The **Sales Invoice** window opens, showing the quantity that you have transferred to the invoice.</span></span>  
9. <span data-ttu-id="ff6a8-131">Apportez les modifications supplémentaires, puis cliquez sur **Valider**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-131">Make any additional changes, and then choose the **Post** action.</span></span>

<span data-ttu-id="ff6a8-132">**Remarque** : La procédure ci-dessus permet également de créer, de consulter, puis de valider un avoir vente associé à un projet.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-132">**Note**: The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.</span></span>

## <a name="to-calculate-and-post-job-completion-entries"></a><span data-ttu-id="ff6a8-133">Pour calculer et valider les écritures d'achèvement du projet</span><span class="sxs-lookup"><span data-stu-id="ff6a8-133">To calculate and post job completion entries</span></span>  
<span data-ttu-id="ff6a8-134">À la fin des activités d'un projet (validation et facturation comprises), vous devez le mettre à jour pour définir le **Statut** du projet sur **Terminé**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-134">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span></span> <span data-ttu-id="ff6a8-135">Ensuite, vous devez contrepasser tous les travaux en cours validés antérieurement dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-135">Then, you must reverse any WIP that has been posted to the general ledger.</span></span>

1. <span data-ttu-id="ff6a8-136">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projets**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-136">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ff6a8-137">Sélectionnez un projet ouvert, puis cliquez sur **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-137">Select an open job, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="ff6a8-138">Dans le champ **Statut**, sélectionnez **Terminé**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-138">In the **Status** field, select **Completed**.</span></span>
4. <span data-ttu-id="ff6a8-139">Suivez les étapes d'aide pour calculer et valider les travaux en cours.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-139">Follow the assistance steps to calculate and post WIP.</span></span> <span data-ttu-id="ff6a8-140">Sinon, suivez les étapes 5 et 6 pour le faire manuellement.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-140">Alternatively, follows steps 5 and 6 to do so manually.</span></span>  
5. <span data-ttu-id="ff6a8-141">Cliquez sur **Calculer TEC**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-141">Choose the **Calculate WIP** action.</span></span>
6. <span data-ttu-id="ff6a8-142">Dans la fenêtre **Projet Calculer TEC**, renseignez les champs comme nécessaire.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-142">In the **Job Calculate WIP** window, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="ff6a8-143">Les écritures TEC projet créées par le traitement par lots auront la case **Projet terminé** cochée pour indiquer qu'il s'agit d'écritures d’achèvement.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-143">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span></span>  

7. <span data-ttu-id="ff6a8-144">Cliquez sur **Projet Valider TEC en comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-144">Choose the **Job Post WIP to G/L** action.</span></span>
8. <span data-ttu-id="ff6a8-145">Dans la fenêtre **Projet Valider TEC en comptabilité**, renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-145">In the **Job Post WIP to G/L** window, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="ff6a8-146">Les écritures comptabilité TEC projet créées par le traitement par lots verront la case **Projet terminé** cochée pour indiquer qu'il s'agit d'écritures d’achèvement.</span><span class="sxs-lookup"><span data-stu-id="ff6a8-146">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span></span>

## <a name="see-also"></a><span data-ttu-id="ff6a8-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ff6a8-147">See Also</span></span>
[<span data-ttu-id="ff6a8-148">Gérer des projets</span><span class="sxs-lookup"><span data-stu-id="ff6a8-148">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="ff6a8-149">Finance</span><span class="sxs-lookup"><span data-stu-id="ff6a8-149">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="ff6a8-150">[Gestion des achats](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="ff6a8-150">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="ff6a8-151">[Gestion des ventes](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="ff6a8-151">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="ff6a8-152">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="ff6a8-152">Work With Dynamics NAV</span></span>](ui-work-product.md)  

