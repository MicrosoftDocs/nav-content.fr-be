---
title: "Procédure : activer les paiements client via Paypal"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a><span data-ttu-id="05e66-102">Procédure : activer les paiements client via PayPal#</span><span class="sxs-lookup"><span data-stu-id="05e66-102">How to: Enable Customer Payments Through PayPal#</span></span>
<span data-ttu-id="05e66-103">Au lieu de collecter des paiements par l'intermédiaire de transferts bancaires ou de cartes de crédit, vous pouvez proposer à vos clients de vous payer via leur compte Paypal.</span><span class="sxs-lookup"><span data-stu-id="05e66-103">As an alternative to collecting payments through bank transfer or credit cards, you can offer your customers to pay you through their PayPal account.</span></span>

<span data-ttu-id="05e66-104">Lorsqu'un client clique sur le lien Paypal sur une facture vente ou un document commande vente, la page de service de leur compte Paypal s'ouvre et affiche les détails de paiement pour la vente.</span><span class="sxs-lookup"><span data-stu-id="05e66-104">When a customer chooses the PayPal link on a sales invoice or sales order document, the service page for their PayPal account appears showing the payment details for the sale.</span></span> <span data-ttu-id="05e66-105">Le client peut ensuite payer la facture comme tout autre paiement Paypal.</span><span class="sxs-lookup"><span data-stu-id="05e66-105">The customer can then pay the invoice as any other PayPal payment.</span></span>

<span data-ttu-id="05e66-106">Pour activer les paiements client via Paypal, vous devez effectuer les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="05e66-106">To enable customer payments through PayPal, you must do the following:</span></span>

1. <span data-ttu-id="05e66-107">Configurer PayPal Payments Standard comme service de paiement dans la fenêtre **Services de paiement**.</span><span class="sxs-lookup"><span data-stu-id="05e66-107">Set up PayPal Payments Standard as a payment service in the **Payments Services** window.</span></span>
2. <span data-ttu-id="05e66-108">Sélectionnez PayPal Payments Standard dans le champ **Service de paiement** du document vente en question.</span><span class="sxs-lookup"><span data-stu-id="05e66-108">Select PayPal Payments Standard in the **Payment Service** field on the sales document in question.</span></span>

<span data-ttu-id="05e66-109">Le service PayPal Payments Standard est installé comme extension de Dynamics NAV et prêt à être activé.</span><span class="sxs-lookup"><span data-stu-id="05e66-109">The PayPal Payments Standard service is installed as an extension to Dynamics NAV and ready to enabled.</span></span> <span data-ttu-id="05e66-110">Pour en savoir plus, voir [Personnalisation de Dynamics NAV à l'aide des extensions ](ui-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="05e66-110">For more information, see [Customizing Dynamics NAV Using Extensions ](ui-extensions.md).</span></span>

## <a name="to-enable-the-paypal-payments-standard-service"></a><span data-ttu-id="05e66-111">Pour activer le service PayPal Payments Standard</span><span class="sxs-lookup"><span data-stu-id="05e66-111">To enable the PayPal Payments Standard service</span></span>
1. <span data-ttu-id="05e66-112">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Services de paiement**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="05e66-112">In the top right corner, choose the **Search for Page or Report** icon, **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="05e66-113">Dans la fenêtre **Services de paiement**, sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="05e66-113">In the **Payment Services** window, choose the **New** action.</span></span>
3. <span data-ttu-id="05e66-114">Sélectionnez **PayPal Standard**, puis fermez la fenêtre.</span><span class="sxs-lookup"><span data-stu-id="05e66-114">Select **PayPal Standard**, and then close the window.</span></span>
4. <span data-ttu-id="05e66-115">Dans la fenêtre **Services de paiement**, sélectionnez l'action **Configuration**.</span><span class="sxs-lookup"><span data-stu-id="05e66-115">In the **Payment Services** window, choose the **Setup** action.</span></span>
5. <span data-ttu-id="05e66-116">Renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="05e66-116">Fill in the fields as necessary.</span></span> <span data-ttu-id="05e66-117">Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="05e66-117">Choose a field to read a short description of the field or link to more information.</span></span>

    <span data-ttu-id="05e66-118">**Remarque** : cochez la case **Toujours inclure dans les documents** si vous souhaitez que le lien hypertexte pour le service de paiement Paypal soit toujours visible sur les documents vente pour lesquels le paiement par Paypal est activé.</span><span class="sxs-lookup"><span data-stu-id="05e66-118">**Note**: Select the **Always Include on Documents** check box if the hyperlink for the PayPal payment service should always be visible on sales documents where payment through PayPal is enabled.</span></span>

6. <span data-ttu-id="05e66-119">Fermez la fenêtre.</span><span class="sxs-lookup"><span data-stu-id="05e66-119">Close the window.</span></span>

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a><span data-ttu-id="05e66-120">Pour sélectionner PayPal Payments Standard sur une facture vente</span><span class="sxs-lookup"><span data-stu-id="05e66-120">To select PayPal Payments Standard on a sales invoice</span></span>
1. <span data-ttu-id="05e66-121">Sur la page d'accueil, sélectionnez **Factures vente**.</span><span class="sxs-lookup"><span data-stu-id="05e66-121">On the Home page, choose **Sales Invoices**.</span></span>
2. <span data-ttu-id="05e66-122">Ouvrez la facture vente pour laquelle vous souhaitez activer les paiements via Paypal.</span><span class="sxs-lookup"><span data-stu-id="05e66-122">Open the sales invoice that you want to enable PayPal payments for.</span></span>
3. <span data-ttu-id="05e66-123">Dans le champ **Service de paiement**, sélectionnez PayPal Payments Standard.</span><span class="sxs-lookup"><span data-stu-id="05e66-123">In the **Payment Service** field, choose PayPal Payments Standard.</span></span>

<span data-ttu-id="05e66-124">**Remarque** : le champ **Service de paiement** est uniquement visible si le service PayPal Payments Standard est activé.</span><span class="sxs-lookup"><span data-stu-id="05e66-124">**Note**: The **Payment Service** field is only visible if the PayPal Payments Standard service is enabled.</span></span>   

## <a name="see-also"></a><span data-ttu-id="05e66-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05e66-125">See Also</span></span>  
[<span data-ttu-id="05e66-126">Configuration des ventes</span><span class="sxs-lookup"><span data-stu-id="05e66-126">Set Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="05e66-127">Gestion des ventes</span><span class="sxs-lookup"><span data-stu-id="05e66-127">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="05e66-128">Personnalisation de Dynamics NAV à l'aide des extensions</span><span class="sxs-lookup"><span data-stu-id="05e66-128">Customizing Dynamics NAV Using Extensions</span></span>](ui-extensions.md)

