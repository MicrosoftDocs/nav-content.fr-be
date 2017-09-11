---
title: "Procédure : Gérer des fournitures de projet"
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
ms.openlocfilehash: 00b9ed8480f6b5ab9265beb0fe2dc0060b1c3192
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-supplies"></a><span data-ttu-id="ede16-102">Procédure : Gérer les fournitures pour un projet</span><span class="sxs-lookup"><span data-stu-id="ede16-102">How to: Manage Job Supplies</span></span>
<span data-ttu-id="ede16-103">La gestion des fournitures des projets relatifs à des articles, services et dépenses est l'un des aspects essentiels de l'exécution d'un projet.</span><span class="sxs-lookup"><span data-stu-id="ede16-103">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="ede16-104">Vous pouvez utiliser les quantités de stock ou effectuer des achats spécifiques au projet en utilisant des commandes achat ou des factures achat.</span><span class="sxs-lookup"><span data-stu-id="ede16-104">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="ede16-105">Par exemple, un projet de service sur un ordinateur requiert un nouveau disque.</span><span class="sxs-lookup"><span data-stu-id="ede16-105">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="ede16-106">Vous devez donc créer une facture achat pour l'acheter et pour enregistrer le projet pour lequel il sera utilisé.</span><span class="sxs-lookup"><span data-stu-id="ede16-106">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="ede16-107">Si le processus d'achat ne requiert pas d'enregistrement séparé de la transaction physique, un achat peut être traité dans la fenêtre **Feuille compta. projet**.</span><span class="sxs-lookup"><span data-stu-id="ede16-107">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window.</span></span> <span data-ttu-id="ede16-108">Pour plus d'informations, reportez-vous à [Procédure : Enregistrer l'utilisation pour les projets](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="ede16-108">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="ede16-109">Pour acheter des articles ou des services pour un projet</span><span class="sxs-lookup"><span data-stu-id="ede16-109">To purchase items or services for a job</span></span>
<span data-ttu-id="ede16-110">La procédure suivante indique comment utiliser une facture achat pour acheter des produits pour un projet.</span><span class="sxs-lookup"><span data-stu-id="ede16-110">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="ede16-111">Les mêmes étapes s'appliquent lors de l'utilisation d'une commande achat.</span><span class="sxs-lookup"><span data-stu-id="ede16-111">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="ede16-112">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Factures achat**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ede16-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ede16-113">Sélectionnez l'action **Nouveau**, puis renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="ede16-113">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="ede16-114">Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="ede16-114">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="ede16-115">Dans les champs **N° projet**</span><span class="sxs-lookup"><span data-stu-id="ede16-115">In the **Job No.**</span></span> <span data-ttu-id="ede16-116">et **N° tâche projet**,</span><span class="sxs-lookup"><span data-stu-id="ede16-116">and **Job Task No.**</span></span> <span data-ttu-id="ede16-117">sélectionnez les informations du projet pour lequel vous souhaitez acheter des articles ou des services.</span><span class="sxs-lookup"><span data-stu-id="ede16-117">fields, select the information of the job that you want to purchase items or services for.</span></span>  

    <span data-ttu-id="ede16-118">La valeur que vous sélectionnez dans le champ **Type ligne projet** définit si une ligne planning est créée lorsque vous validez l'activité de l'article.</span><span class="sxs-lookup"><span data-stu-id="ede16-118">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="ede16-119">Si le champ indique **Facturable**, les lignes planning projet prêtes pour facturation sont créées.</span><span class="sxs-lookup"><span data-stu-id="ede16-119">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="ede16-120">Pour plus d'informations, reportez-vous à [Procédure : Facturer des projets](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="ede16-120">For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).</span></span>

4. <span data-ttu-id="ede16-121">Sélectionnez l'action **Valider**.</span><span class="sxs-lookup"><span data-stu-id="ede16-121">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="ede16-122">Pour afficher la valeur des achats pour un projet</span><span class="sxs-lookup"><span data-stu-id="ede16-122">To view the value of purchases for a job</span></span>  

1. <span data-ttu-id="ede16-123">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projets**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ede16-123">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="ede16-124">Ouvrez la fiche projet appropriée.</span><span class="sxs-lookup"><span data-stu-id="ede16-124">Open a relevant job card.</span></span>

    <span data-ttu-id="ede16-125">Dans le raccourci **Tâches**, le champ **Commandes ouvertes** affiche le montant total en commande, en devise société, des articles en stock et des services sur les documents achat pour la tâche projet ligne.</span><span class="sxs-lookup"><span data-stu-id="ede16-125">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="ede16-126">Le champ **Montant reçu non facturé** affiche la valeur des articles livrés sur les documents achat mais non facturés.</span><span class="sxs-lookup"><span data-stu-id="ede16-126">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  

3. <span data-ttu-id="ede16-127">Choisissez l'un des champs pour ouvrir la fenêtre **Lignes achat** dans laquelle vous pouvez consulter des informations sur les lignes de document achat associées, incluant les articles ou les services qui ont été réceptionnés.</span><span class="sxs-lookup"><span data-stu-id="ede16-127">Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="ede16-128">Pour valider des frais liés à un projet</span><span class="sxs-lookup"><span data-stu-id="ede16-128">To post a job-related expense</span></span>  
<span data-ttu-id="ede16-129">Si vous supportez les dépenses extraordinaires ou exceptionnelles du projet, vous pouvez utiliser la fenêtre **Feuille compta. projet** pour les valider directement dans le compte projet approprié.</span><span class="sxs-lookup"><span data-stu-id="ede16-129">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="ede16-130">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Feuilles compta. projet**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ede16-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ede16-131">Créez une ligne et renseignez les informations concernant les frais, notamment les informations des champs **N° projet**</span><span class="sxs-lookup"><span data-stu-id="ede16-131">Create a new line and enter information about the expense, including information in the **Job No.**</span></span> <span data-ttu-id="ede16-132">et **N° tâche projet**.</span><span class="sxs-lookup"><span data-stu-id="ede16-132">and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="ede16-133">Lorsque la feuille est renseignée, cliquez sur **Valider**.</span><span class="sxs-lookup"><span data-stu-id="ede16-133">When the journal is complete, choose the **Post** action.</span></span>


## <a name="see-also"></a><span data-ttu-id="ede16-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ede16-134">See Also</span></span>
[<span data-ttu-id="ede16-135">Gérer des projets</span><span class="sxs-lookup"><span data-stu-id="ede16-135">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="ede16-136">Finance</span><span class="sxs-lookup"><span data-stu-id="ede16-136">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="ede16-137">[Gestion des achats](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="ede16-137">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="ede16-138">[Gestion des ventes](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="ede16-138">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="ede16-139">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="ede16-139">Work With Dynamics NAV</span></span>](ui-work-product.md)  

