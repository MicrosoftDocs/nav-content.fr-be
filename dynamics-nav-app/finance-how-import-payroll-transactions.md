---
title: "Procédure d'importation de transactions de paie "
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d5e70a0a1659c7facdeec3f0971eda43ff8a03cc
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-import-payroll-transactions"></a><span data-ttu-id="61a6a-102">Procédure d'importation de transactions de paie </span><span class="sxs-lookup"><span data-stu-id="61a6a-102">How to: Import Payroll Transactions</span></span>
<span data-ttu-id="61a6a-103">Pour tenir compte des paiements des salaires et des transactions associées, vous devez importer et valider des transactions financières effectuées par votre fournisseur de paie dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="61a6a-103">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span> <span data-ttu-id="61a6a-104">Pour cela, vous devez tout d'abord importer un fichier csv.</span><span class="sxs-lookup"><span data-stu-id="61a6a-104">To do this, you first import a csv.</span></span> <span data-ttu-id="61a6a-105">que vous recevez du fournisseur de paie dans la fenêtre **Feuille comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="61a6a-105">file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="61a6a-106">Vous devez ensuite mapper les comptes externes du fichier de paie aux comptes généraux appropriés.</span><span class="sxs-lookup"><span data-stu-id="61a6a-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="61a6a-107">Enfin, vous devez valider les transactions de paie en fonction du mappage de compte.</span><span class="sxs-lookup"><span data-stu-id="61a6a-107">Lastly, you post the payroll transactions according to the account mapping.</span></span>

## <a name="to-import-a-payroll-file"></a><span data-ttu-id="61a6a-108">Pour importer un fichier de paie</span><span class="sxs-lookup"><span data-stu-id="61a6a-108">To import a payroll file</span></span>
1. <span data-ttu-id="61a6a-109">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuilles comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="61a6a-109">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="61a6a-110">Dans le nom feuille comptabilité pertinent, sélectionnez l'action **Importer les transactions de paie**.</span><span class="sxs-lookup"><span data-stu-id="61a6a-110">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span></span>
3. <span data-ttu-id="61a6a-111">Dans la fenêtre **Importer**, sélectionnez le fichier de paie qui convient, puis cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="61a6a-111">In the **Import** window, select the relevant payroll file, and then choose the **OK** button.</span></span> <span data-ttu-id="61a6a-112">Le fichier doit être au format CSV.</span><span class="sxs-lookup"><span data-stu-id="61a6a-112">The file must be in CSV format.</span></span> 
4. <span data-ttu-id="61a6a-113">Suivez les étapes de la fenêtre **Importer les transactions de paie** pour importer les transactions et mapper les comptes, puis cliquez sur le bouton **Terminer**.</span><span class="sxs-lookup"><span data-stu-id="61a6a-113">Follow the steps in the **Import Payroll Transactions** window to import transactions and map accounts, and then choose the **Finish** button.</span></span>

    <span data-ttu-id="61a6a-114">La feuille comptabilité est complétée par des lignes représentant les transactions contenues dans le fichier de paie et par les comptes appropriés de la colonne **Compte général**.</span><span class="sxs-lookup"><span data-stu-id="61a6a-114">The general journal is filled with lines representing the transactions that the payroll file contains and with the relevant accounts in the **G/L Account** column.</span></span>
4. <span data-ttu-id="61a6a-115">Modifiez ou validez les lignes feuille comme pour toute autre transaction comptable générale.</span><span class="sxs-lookup"><span data-stu-id="61a6a-115">Edit or post the journal lines as for any other general ledger transactions.</span></span> <span data-ttu-id="61a6a-116">Pour plus d'informations, reportez-vous à [Procédure : utilisation des feuilles comptabilité](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="61a6a-116">For more information, see [How to: Work With General Journals](ui-work-general-journals.md).</span></span>   

## <a name="see-also"></a><span data-ttu-id="61a6a-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="61a6a-117">See Also</span></span>
[<span data-ttu-id="61a6a-118">Finance</span><span class="sxs-lookup"><span data-stu-id="61a6a-118">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="61a6a-119">Procédure : travailler avec les feuilles comptabilité</span><span class="sxs-lookup"><span data-stu-id="61a6a-119">How to: Work With General Journals</span></span>](ui-work-general-journals.md)  

