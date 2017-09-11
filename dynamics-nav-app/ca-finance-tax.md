---
title: Taxe sur les ventes et taxe sur les biens et les services au Canada
author: edupont04
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c032a02b545441b927ef5c4facc9f77731f37ab7
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-goods-and-services-tax-in-canada"></a><span data-ttu-id="ee602-102">Taxe sur les ventes et taxe sur les biens et les services au Canada</span><span class="sxs-lookup"><span data-stu-id="ee602-102">Sales Tax and Goods and Services Tax in Canada</span></span>
<span data-ttu-id="ee602-103">Au Canada, si un fournisseur n'a pas de présence commerciale dans la province dans laquelle les achats sont effectués, le fournisseur facture la taxe sur les biens et des services (Goods and Services Tax - GST) ou la taxe harmonisée (Harmonized Sales Tax - HST) uniquement.</span><span class="sxs-lookup"><span data-stu-id="ee602-103">In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only.</span></span> <span data-ttu-id="ee602-104">Toutefois, si la province applique une taxe provinciale sur les ventes (Provincial Sales Tax - PST), l'acheteur doit tout de même calculer le montant de la PST et le payer directement à la province.</span><span class="sxs-lookup"><span data-stu-id="ee602-104">However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province.</span></span> <span data-ttu-id="ee602-105">Lorsqu'un code zone de recouvrement provincial est sélectionné, Dynamics NAV l'utilise pour calculer la PST et la valider de sorte que l'impôt à payer apparaisse à la fois dans la comptabilité et dans les enregistrement d'écriture TVA.</span><span class="sxs-lookup"><span data-stu-id="ee602-105">When a Provincial Tax Area Code is selected, Dynamics NAV uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records.</span></span> <span data-ttu-id="ee602-106">Par conséquent, le code zone de recouvrement sélectionné ici doit uniquement inclure la PST et non la GST.</span><span class="sxs-lookup"><span data-stu-id="ee602-106">Therefore, the tax area code selected here should be one where only the PST is included, not the GST.</span></span>  
<span data-ttu-id="ee602-107">Pour plus d'informations de la taxe sur les ventes, reportez-vous à [Taxe sur les ventes et groupes de taxes aux États-Unis et au Canada](us-finance-setup-sales-tax.md).</span><span class="sxs-lookup"><span data-stu-id="ee602-107">For more information about sales tax, see [Sales Tax and Tax Groups in the US and Canada](us-finance-setup-sales-tax.md).</span></span>  

## <a name="submitting-the-gsthst-file"></a><span data-ttu-id="ee602-108">Envoi du fichier GST/HST</span><span class="sxs-lookup"><span data-stu-id="ee602-108">Submitting the GST/HST File</span></span>
<span data-ttu-id="ee602-109">Les informations sur les taxes dans les documents achat permettent de générer un transfert de fichier GST/HST par Internet, fichier que vous devez transmettre aux autorités fiscales.</span><span class="sxs-lookup"><span data-stu-id="ee602-109">The tax information in purchase documents is used to generate a GST/HST internet file transfer that you must  provided to the tax authorities.</span></span> <span data-ttu-id="ee602-110">Ce champ inclut la taxe sur les biens et les services (GST) et la taxe harmonisée (HST).</span><span class="sxs-lookup"><span data-stu-id="ee602-110">This file includes goods and services tax (GST) and harmonized sales tax (HST).</span></span> <span data-ttu-id="ee602-111">Le fichier est créé dans un format de fichier .tax, qui peut être transféré via Internet.</span><span class="sxs-lookup"><span data-stu-id="ee602-111">The file is created in a .tax file format, which can be transferred via the internet.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ee602-112">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ee602-112">See Also</span></span>
[<span data-ttu-id="ee602-113">Finance</span><span class="sxs-lookup"><span data-stu-id="ee602-113">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="ee602-114">Configuration de la finance</span><span class="sxs-lookup"><span data-stu-id="ee602-114">Set Up Finance</span></span>](finance-setup-setup-finance-setup.md)  
[<span data-ttu-id="ee602-115">Taxe sur les ventes et groupes de taxes aux États-Unis et au Canada</span><span class="sxs-lookup"><span data-stu-id="ee602-115">Sales Tax and Tax Groups in the US and Canada</span></span>](us-finance-setup-sales-tax.md)

