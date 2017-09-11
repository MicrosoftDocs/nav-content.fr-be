---
title: Configuration ou modification du plan comptable
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 2a2f1f2ec3ac5bdd935ec19c11d74e16bdee7686
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a><span data-ttu-id="5eab4-102">Configuration ou modification du plan comptable</span><span class="sxs-lookup"><span data-stu-id="5eab4-102">Set Up or Change the Chart of Accounts</span></span>
<span data-ttu-id="5eab4-103">Le plan comptable affiche les comptes généraux qui stockent vos données financières.</span><span class="sxs-lookup"><span data-stu-id="5eab4-103">The chart of accounts shows the ledger accounts that store your financial data.</span></span> <span data-ttu-id="5eab4-104">Dynamics NAV inclut un plan comptable standard prêt à prendre en charge votre société.</span><span class="sxs-lookup"><span data-stu-id="5eab4-104">Dynamics NAV includes a standard chart of accounts that is ready to support your business.</span></span>
<span data-ttu-id="5eab4-105">Cependant, vous pouvez modifier les comptes par défaut, et vous pouvez ajouter de nouveaux comptes.</span><span class="sxs-lookup"><span data-stu-id="5eab4-105">However, you can change the default accounts, and you can add new accounts.</span></span>  

## <a name="adding-or-changing-accounts"></a><span data-ttu-id="5eab4-106">Ajout ou modification de comptes</span><span class="sxs-lookup"><span data-stu-id="5eab4-106">Adding or Changing Accounts</span></span>
<span data-ttu-id="5eab4-107">À partir du plan comptable, vous pouvez ouvrir chaque compte général et ajouter ou modifier des paramètres.</span><span class="sxs-lookup"><span data-stu-id="5eab4-107">From the chart of accounts, you can open each G/L account and add or change settings.</span></span>

<span data-ttu-id="5eab4-108">**Remarque** : vous pouvez supprimer un compte général.</span><span class="sxs-lookup"><span data-stu-id="5eab4-108">**Note**: You can delete a general ledger account.</span></span> <span data-ttu-id="5eab4-109">Toutefois, avant que de le supprimer, les conditions suivantes doivent être réunies :</span><span class="sxs-lookup"><span data-stu-id="5eab4-109">However, before you delete it, the following must be true:</span></span>  
- <span data-ttu-id="5eab4-110">Le solde du compte doit être nul.</span><span class="sxs-lookup"><span data-stu-id="5eab4-110">The balance on the account must be zero.</span></span>  
- <span data-ttu-id="5eab4-111">Le champ **Autoriser suppr. cpte gén. av.** doit être défini dans la fenêtre **Paramètres comptabilité**, et le compte ne doit pas comporter d'écritures comptables à cette date ou après celle-ci.</span><span class="sxs-lookup"><span data-stu-id="5eab4-111">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span></span>  
- <span data-ttu-id="5eab4-112">Si le champ **Vérifier activité cpte général** de la fenêtre **Paramètres comptabilité** est sélectionné, le compte ne doit pas être utilisé dans les groupes comptabilisation ni dans une configuration de la validation.</span><span class="sxs-lookup"><span data-stu-id="5eab4-112">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span></span>  

<span data-ttu-id="5eab4-113">Dynamics NAV vous empêchera de supprimer un compte général qui stocke les données nécessaires au plan comptable.</span><span class="sxs-lookup"><span data-stu-id="5eab4-113">Dynamics NAV will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span></span>  

##<a name="see-also"></a><span data-ttu-id="5eab4-114">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5eab4-114">See Also</span></span>  
[<span data-ttu-id="5eab4-115">Les écritures comptables et le plan comptable</span><span class="sxs-lookup"><span data-stu-id="5eab4-115">The General Ledger and the Chart of Accounts</span></span>](finance-setup-general-ledger.md)  
[<span data-ttu-id="5eab4-116">Gérer les comptes bancaires</span><span class="sxs-lookup"><span data-stu-id="5eab4-116">Manage Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="5eab4-117">Axes analytiques</span><span class="sxs-lookup"><span data-stu-id="5eab4-117">Dimensions</span></span>](finance-setup-dimensions.md)  
[<span data-ttu-id="5eab4-118">Procédure : utilisation des codes IGRF au Canada</span><span class="sxs-lookup"><span data-stu-id="5eab4-118">How to: Work With GIFI Codes in Canada</span></span>](ca-finance-setup-work-GiFI-codes.md)

