---
title: Comment charger les fichiers paiement sur un serveur Isabel
description: "Les fichiers paiement peuvent être chargés à l'aide de la fenêtre **Journaux IBS**. Les champs **Mode d'intégration du téléchargement (amont)** et **Mode d'intégration du téléchargement (aval)** dans la fenêtre **Configuration de la banque électronique** doivent être définis sur **Interactif** pour charger des fichiers paiement."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d9d62008d1e3c2923d9640e3997b31ab95e76dc4
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-upload-payment-files-to-an-isabel-server"></a><span data-ttu-id="279c1-104">Comment charger les fichiers paiement sur un serveur Isabel</span><span class="sxs-lookup"><span data-stu-id="279c1-104">How to: Upload Payment Files to an Isabel Server</span></span>
<span data-ttu-id="279c1-105">Les fichiers paiement peuvent être chargés à l'aide de la fenêtre **Journaux IBS**.</span><span class="sxs-lookup"><span data-stu-id="279c1-105">Payment files can be uploaded using the **IBS Logs** window.</span></span> <span data-ttu-id="279c1-106">Les champs **Mode d'intégration du téléchargement (amont)** et **Mode d'intégration du téléchargement (aval)** dans la fenêtre **Configuration de la banque électronique** doivent être définis sur **Interactif** pour charger des fichiers paiement.</span><span class="sxs-lookup"><span data-stu-id="279c1-106">The **Upload Integration Mode** and **Download Integration Mode** fields in the **Electronic Banking Setup** window must be set to **Attended** to upload payment files.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="279c1-107">Avant de pouvoir charger des fichiers paiement, vous devez vous connecter au serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="279c1-107">Before you can upload payment files you must be logged on to the Isabel server.</span></span>  
  
### <a name="to-upload-payment-files-in-attended-mode"></a><span data-ttu-id="279c1-108">Pour charger des fichiers paiement en mode interactif</span><span class="sxs-lookup"><span data-stu-id="279c1-108">To upload payment files in attended mode</span></span>  
  
1.  <span data-ttu-id="279c1-109">Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Journaux IBS**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="279c1-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **IBS Logs**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="279c1-110">Dans l'onglet **Accueil**, dans le groupe **Processus**, sélectionnez **Extraire le contrat et l'utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="279c1-110">On the **Home** tab, in the **Process** group, choose **Get Contract and User**.</span></span>  
  
3.  <span data-ttu-id="279c1-111">Une fois les fichiers paiement vérifiés, un code utilisateur et un ID contrat s'afficheront dans les champs **Code utilisateur IBS** et **ID contrat IBS**.</span><span class="sxs-lookup"><span data-stu-id="279c1-111">After verifying the payment files, a user ID and contract ID will be displayed in the **IBS User ID** and **IBS Contract ID** fields.</span></span>  
  
     <span data-ttu-id="279c1-112">Le champ **Statut du téléchargement** sera défini sur **Prêt pour téléchargement**.</span><span class="sxs-lookup"><span data-stu-id="279c1-112">The **Upload Status** field will be set to **Ready for Upload**.</span></span> <span data-ttu-id="279c1-113">S'il existe plus d'un contrat sur le serveur Isabel pour le compte bancaire, le champ **Statut du téléchargement** sera défini sur **Existence d'un conflit**.</span><span class="sxs-lookup"><span data-stu-id="279c1-113">If more than one contract exists on the Isabel server for the bank account, the **Upload Status** will be set to **Conflict Exists**.</span></span> <span data-ttu-id="279c1-114">Sélectionnez le contrat adéquat.</span><span class="sxs-lookup"><span data-stu-id="279c1-114">Select the correct contract.</span></span>  
  
4.  <span data-ttu-id="279c1-115">Dans l'onglet **Accueil**, dans le groupe **Traiter**, sélectionnez **Procéder au téléchargement**.</span><span class="sxs-lookup"><span data-stu-id="279c1-115">On the **Home** tab, in the **Process** group, choose **Perform Download**.</span></span> <span data-ttu-id="279c1-116">Les fichiers paiement seront téléchargés sur le serveur Isabel et le champ **Statut du téléchargement** sera défini sur **Traité**.</span><span class="sxs-lookup"><span data-stu-id="279c1-116">The payment files will be uploaded to the Isabel server and the **Process Status** field will be set to **Processed**.</span></span>  
  
5.  <span data-ttu-id="279c1-117">Continuez à traiter les fichiers paiement en signant et en envoyant les fichiers sur le serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="279c1-117">Continue processing the payment files by signing and sending the files on the Isabel server.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="279c1-118">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="279c1-118">See Also</span></span>  
 <span data-ttu-id="279c1-119">Configuration de la banque électronique</span><span class="sxs-lookup"><span data-stu-id="279c1-119">Electronic Banking Setup</span></span>   
 <span data-ttu-id="279c1-120">Journaux IBS</span><span class="sxs-lookup"><span data-stu-id="279c1-120">IBS Logs</span></span>   
 [<span data-ttu-id="279c1-121">Comment archiver les écritures journal IBS</span><span class="sxs-lookup"><span data-stu-id="279c1-121">How to: Archive IBS Log Entries</span></span>](how-to-archive-ibs-log-entries.md)
