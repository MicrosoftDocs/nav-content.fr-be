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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: fa15bbba7beb1a90df5a6051ab763a802268da79
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-upload-payment-files-to-an-isabel-server"></a><span data-ttu-id="553f7-104">Comment charger les fichiers paiement sur un serveur Isabel</span><span class="sxs-lookup"><span data-stu-id="553f7-104">How to: Upload Payment Files to an Isabel Server</span></span>
<span data-ttu-id="553f7-105">Les fichiers paiement peuvent être chargés à l'aide de la fenêtre **Journaux IBS**.</span><span class="sxs-lookup"><span data-stu-id="553f7-105">Payment files can be uploaded using the **IBS Logs** window.</span></span> <span data-ttu-id="553f7-106">Les champs **Mode d'intégration du téléchargement (amont)** et **Mode d'intégration du téléchargement (aval)** dans la fenêtre **Configuration de la banque électronique** doivent être définis sur **Interactif** pour charger des fichiers paiement.</span><span class="sxs-lookup"><span data-stu-id="553f7-106">The **Upload Integration Mode** and **Download Integration Mode** fields in the **Electronic Banking Setup** window must be set to **Attended** to upload payment files.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="553f7-107">Avant de pouvoir charger des fichiers paiement, vous devez vous connecter au serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="553f7-107">Before you can upload payment files you must be logged on to the Isabel server.</span></span>  

## <a name="to-upload-payment-files-in-attended-mode"></a><span data-ttu-id="553f7-108">Pour charger des fichiers paiement en mode interactif</span><span class="sxs-lookup"><span data-stu-id="553f7-108">To upload payment files in attended mode</span></span>  

1.  <span data-ttu-id="553f7-109">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Journaux IBS**, puis sélectionnez le lien correspondant.</span><span class="sxs-lookup"><span data-stu-id="553f7-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **IBS Logs**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="553f7-110">Choisissez l'action **Extraire le contrat et l'utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="553f7-110">Choose the **Get Contract and User** action.</span></span>  
3.  <span data-ttu-id="553f7-111">Une fois les fichiers paiement vérifiés, un code utilisateur et un ID contrat s'afficheront dans les champs **Code utilisateur IBS** et **ID contrat IBS**.</span><span class="sxs-lookup"><span data-stu-id="553f7-111">After verifying the payment files, a user ID and contract ID will be displayed in the **IBS User ID** and **IBS Contract ID** fields.</span></span>  

    <span data-ttu-id="553f7-112">Le champ **Statut du téléchargement** sera défini sur **Prêt pour téléchargement**.</span><span class="sxs-lookup"><span data-stu-id="553f7-112">The **Upload Status** field will be set to **Ready for Upload**.</span></span> <span data-ttu-id="553f7-113">S'il existe plus d'un contrat sur le serveur Isabel pour le compte bancaire, le champ **Statut du téléchargement** sera défini sur **Existence d'un conflit**.</span><span class="sxs-lookup"><span data-stu-id="553f7-113">If more than one contract exists on the Isabel server for the bank account, the **Upload Status** will be set to **Conflict Exists**.</span></span> <span data-ttu-id="553f7-114">Sélectionnez le contrat adéquat.</span><span class="sxs-lookup"><span data-stu-id="553f7-114">Select the correct contract.</span></span>  

4.  <span data-ttu-id="553f7-115">Choisissez l'action **Procéder au téléchargement**.</span><span class="sxs-lookup"><span data-stu-id="553f7-115">Choose the **Perform Download** action.</span></span> <span data-ttu-id="553f7-116">Les fichiers paiement seront téléchargés sur le serveur Isabel et le champ **Statut du téléchargement** sera défini sur **Traité**.</span><span class="sxs-lookup"><span data-stu-id="553f7-116">The payment files will be uploaded to the Isabel server and the **Process Status** field will be set to **Processed**.</span></span>  
5.  <span data-ttu-id="553f7-117">Continuez à traiter les fichiers paiement en signant et en envoyant les fichiers sur le serveur Isabel.</span><span class="sxs-lookup"><span data-stu-id="553f7-117">Continue processing the payment files by signing and sending the files on the Isabel server.</span></span>  

## <a name="see-also"></a><span data-ttu-id="553f7-118">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="553f7-118">See Also</span></span>  
 [<span data-ttu-id="553f7-119">Comment archiver les écritures journal IBS</span><span class="sxs-lookup"><span data-stu-id="553f7-119">How to: Archive IBS Log Entries</span></span>](how-to-archive-ibs-log-entries.md)

