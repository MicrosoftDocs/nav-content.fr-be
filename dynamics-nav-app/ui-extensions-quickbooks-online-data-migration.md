---
title: Utilisation de l'extension QuickBooks Data Migration
description: "Décrit comment utiliser l'extension pour migrer des clients, des fournisseurs, des articles, et des comptes de QuickBooks Online à Dynamics NAV."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, QuickBooks, import
ms.date: 05/24/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ff8f8f0c529966fc108d2d4c86e2d0681b1fc005
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---

# <a name="the-quickbooks-online-data-migration-extension-for-dynamics-nav"></a><span data-ttu-id="20397-103">L'extension QuickBooks Online Data Migration pour Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="20397-103">The QuickBooks Online Data Migration Extension for Dynamics NAV</span></span>
<span data-ttu-id="20397-104">Cette extension est incluse dans le guide d'installation facilité **Migration des données** pour vous aider à migrer les données métier pertinentes de QuickBooks Online vers [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="20397-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="20397-105">Par exemple, c'est utile si votre activité se développe, et que vous avez décidé de mettre à niveau votre application de gestion d'entreprise en commençant à utiliser [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="20397-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="what-data-can-i-import-from-quickbooks-online"></a><span data-ttu-id="20397-106">Quelles données puis-je importer de QuickBooks Online ?</span><span class="sxs-lookup"><span data-stu-id="20397-106">What data can I import from QuickBooks Online?</span></span>
<span data-ttu-id="20397-107">Vous pouvez importer les données suivantes de QuickBooks Online vers [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="20397-107">You can import the following data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

* <span data-ttu-id="20397-108">Clients</span><span class="sxs-lookup"><span data-stu-id="20397-108">Customers</span></span>
* <span data-ttu-id="20397-109">Fournisseurs</span><span class="sxs-lookup"><span data-stu-id="20397-109">Vendors</span></span>
* <span data-ttu-id="20397-110">Articles</span><span class="sxs-lookup"><span data-stu-id="20397-110">Items</span></span>
* <span data-ttu-id="20397-111">Plan comptable</span><span class="sxs-lookup"><span data-stu-id="20397-111">Chart of accounts</span></span> 
* <span data-ttu-id="20397-112">Commencer la transaction de solde en comptabilité</span><span class="sxs-lookup"><span data-stu-id="20397-112">Beginning balance transaction in the general ledger</span></span>
* <span data-ttu-id="20397-113">Quantités disponibles pour les articles de stock</span><span class="sxs-lookup"><span data-stu-id="20397-113">On-hand quantities for inventory items</span></span>
* <span data-ttu-id="20397-114">Ouvrir des documents pour les clients et les fournisseurs, par exemple des factures, des avoirs, et des paiements</span><span class="sxs-lookup"><span data-stu-id="20397-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span></span>

<span data-ttu-id="20397-115">Nous effectuons une migration uniquement pour les montants complets dans les documents achat et vente.</span><span class="sxs-lookup"><span data-stu-id="20397-115">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="20397-116">Nous ne mettons pas à jour les montants partiellement payés.</span><span class="sxs-lookup"><span data-stu-id="20397-116">We do not update partially paid amounts.</span></span> <span data-ttu-id="20397-117">Par exemple, si un client a payé 300 dollars sur un total de 500 dollars dans une facture vente, nous effectuons une migration des 500 complets.</span><span class="sxs-lookup"><span data-stu-id="20397-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="20397-118">Si vous avez reçu des paiements partiels, vous devez les mettre à jour manuellement, avant ou après la migration de données.</span><span class="sxs-lookup"><span data-stu-id="20397-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="20397-119">Nous vous recommandons de lettrer les transactions ouvertes avant d'exécuter une migration, pour faciliter juste des éléments ensuite.</span><span class="sxs-lookup"><span data-stu-id="20397-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]  
>   <span data-ttu-id="20397-120">Nous n'effectuons pas de migration des commandes achat ou des commandes vente.</span><span class="sxs-lookup"><span data-stu-id="20397-120">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="20397-121">Avant de commencer</span><span class="sxs-lookup"><span data-stu-id="20397-121">Before you start</span></span>
<span data-ttu-id="20397-122">Une grande partie du processus de migration consiste à spécifier les comptes vers lesquels migrer les transactions.</span><span class="sxs-lookup"><span data-stu-id="20397-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="20397-123">Il est judicieux de planifier ce mappage avant d'exécuter la migration de données.</span><span class="sxs-lookup"><span data-stu-id="20397-123">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="20397-124">Par exemple, les comptes où vous validez des transactions :</span><span class="sxs-lookup"><span data-stu-id="20397-124">For example, the accounts where you post transactions for:</span></span>  
  
* <span data-ttu-id="20397-125">La vente d'articles ou de services à un client.</span><span class="sxs-lookup"><span data-stu-id="20397-125">The sale of items or services to customers.</span></span>
* <span data-ttu-id="20397-126">L'achat d'articles ou de service auprès d'un fournisseur.</span><span class="sxs-lookup"><span data-stu-id="20397-126">The purchase of items or services from vendors.</span></span>  
* <span data-ttu-id="20397-127">Ajustements des écritures comptables.</span><span class="sxs-lookup"><span data-stu-id="20397-127">Adjustments in the general ledger.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="20397-128"> nécessite que les comptes généraux aient des numéros de compte.</span><span class="sxs-lookup"><span data-stu-id="20397-128"> requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="20397-129">S'assurer que les numéros de compte sont affectés aux comptes dans QuickBooks Online.</span><span class="sxs-lookup"><span data-stu-id="20397-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span></span>

<span data-ttu-id="20397-130">Si les transactions de QuickBooks Online ont des montants de taxe, vous devez créer un compte taxes pour vos administrations fiscales dans [!INCLUDE[d365fin](includes/d365fin_md.md)] avant de pouvoir valider des transactions.</span><span class="sxs-lookup"><span data-stu-id="20397-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you can post transactions.</span></span>

## <a name="how-do-i-start-using-the-extension"></a><span data-ttu-id="20397-131">Comment commencer à utiliser à l'extension ?</span><span class="sxs-lookup"><span data-stu-id="20397-131">How do I start using the extension?</span></span>
<span data-ttu-id="20397-132">La mise en route est simple.</span><span class="sxs-lookup"><span data-stu-id="20397-132">Getting started is easy.</span></span> <span data-ttu-id="20397-133">Il vous suffit d'exécuter le guide d'installation assistée **Migration des données**.</span><span class="sxs-lookup"><span data-stu-id="20397-133">All you need to do is run the **Data Migration** assisted setup guide.</span></span> <span data-ttu-id="20397-134">Voici comment :</span><span class="sxs-lookup"><span data-stu-id="20397-134">Here's how:</span></span>

1. <span data-ttu-id="20397-135">Choisissez l'icône ![Page ou état pour la recherchei](media/ui-search/search_small.png "cône Page ou état pour la recherche") et entrez **Configuration assistée**, puis **Migrer des données métier**.</span><span class="sxs-lookup"><span data-stu-id="20397-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span></span>
2. <span data-ttu-id="20397-136">Suivez les instructions à chaque étape du guide d'installation assistée.</span><span class="sxs-lookup"><span data-stu-id="20397-136">Follow the instructions on each step in the assisted setup guide.</span></span>

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="20397-137">Que faire après une migration des données ?</span><span class="sxs-lookup"><span data-stu-id="20397-137">What do I do after I migrate data?</span></span>
<span data-ttu-id="20397-138">Après avoir effectué une migration des données, les transactions ont le statut **Non validé**, vous pouvez les consulter et faire des ajustements.</span><span class="sxs-lookup"><span data-stu-id="20397-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span></span> <span data-ttu-id="20397-139">Pour consulter les transactions, accédez à la page où vous les trouveriez normalement.</span><span class="sxs-lookup"><span data-stu-id="20397-139">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="20397-140">Par exemple, pour examiner les factures vente non validées, accédez à la page **Factures vente**.</span><span class="sxs-lookup"><span data-stu-id="20397-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span></span> <span data-ttu-id="20397-141">Pour consulter des feuilles paiement, accédez à la page **Feuilles paiement**.</span><span class="sxs-lookup"><span data-stu-id="20397-141">To review payment journals, go to the **Payment Journals** page.</span></span>   

<span data-ttu-id="20397-142">Il existe quelques éléments en particulier que vous devez effectuer :</span><span class="sxs-lookup"><span data-stu-id="20397-142">There are a few things in particular that you should do:</span></span>

* <span data-ttu-id="20397-143">Si les transactions dans QuickBooks Online avaient des montants de majoration ou remise, vous devez ajouter manuellement les montants aux transactions associées dans [!INCLUDE[d365fin](includes/d365fin_md.md)] avant de les valider.</span><span class="sxs-lookup"><span data-stu-id="20397-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you post them.</span></span>
* <span data-ttu-id="20397-144">Si vous utilisez la taxe sur la valeur ajoutée (TVA), vous devez ajouter un groupe comptabilisation marché et un groupe comptabilisation produit au paramétrage de la validation de manière à pouvoir valider les montants TVA.</span><span class="sxs-lookup"><span data-stu-id="20397-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
* <span data-ttu-id="20397-145">Vérifiez les soldes de début des comptes du grand livre.</span><span class="sxs-lookup"><span data-stu-id="20397-145">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="20397-146">QuickBooks Online ne stocke pas le solde actuel de tous les comptes, vous pouvez être amené à corriger les soldes d'ouverture.</span><span class="sxs-lookup"><span data-stu-id="20397-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="20397-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20397-147">See Also</span></span>
[<span data-ttu-id="20397-148">Importation des données métier à partir d'autres systèmes financiers</span><span class="sxs-lookup"><span data-stu-id="20397-148">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="20397-149">[Personnalisation de [!INCLUDE[d365fin](includes/d365fin_md.md)] à l'aide des extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="20397-149">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
