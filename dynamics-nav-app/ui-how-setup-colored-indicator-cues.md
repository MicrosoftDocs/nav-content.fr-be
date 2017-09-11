---
title: "Procédure : configurer un indicateur coloré sur des piles"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 38cd904d0cf22374eac430d035e6ea6d205bcab8
ms.contentlocale: fr-be
ms.lasthandoff: 07/19/2017

---
    
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a><span data-ttu-id="29e7d-102">Procédure : configurer un indicateur coloré sur des piles</span><span class="sxs-lookup"><span data-stu-id="29e7d-102">How to: Set Up a Colored Indicator on Cues</span></span>
<span data-ttu-id="29e7d-103">Vous pouvez configurer des piles qui apparaissent sur la page **Accueil** afin d'inclure un indicateur qui change de couleur en fonction des valeurs de données dans les piles.</span><span class="sxs-lookup"><span data-stu-id="29e7d-103">You can set up Cues that appear on the **Home** page to include an indicator that changes color based on the data values in the Cues.</span></span> 

<span data-ttu-id="29e7d-104">L'indicateur apparait sous forme d'une barre de couleur le long de la bordure supérieure de la mosaïque Pile.</span><span class="sxs-lookup"><span data-stu-id="29e7d-104">The indicator appears as a colored bar along the top border of the Cue tile.</span></span> <span data-ttu-id="29e7d-105">Il offre un signal visuel du statut de l'activité de la pile, ce qui peut indiquer des conditions favorables ou défavorables pour inviter l'utilisateur à prendre des mesures.</span><span class="sxs-lookup"><span data-stu-id="29e7d-105">It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action.</span></span> <span data-ttu-id="29e7d-106">Par exemple, si une pile affiche les factures vente en cours, vous pouvez définir l'indicateur pour qu'il apparaisse vert (favorable) lorsque le nombre total des factures vente en cours est inférieur à 10, et apparaisse rouge (défavorable) lorsque le total est supérieur à 20.</span><span class="sxs-lookup"><span data-stu-id="29e7d-106">For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.</span></span>

<span data-ttu-id="29e7d-107">Dans la fenêtre **Paramètres pile**, vous configurez des indicateurs pour toutes les piles disponibles dans la base de données de la société.</span><span class="sxs-lookup"><span data-stu-id="29e7d-107">From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.</span></span>

<span data-ttu-id="29e7d-108">Pour configurer l'indicateur, vous pouvez spécifier jusqu'à deux valeurs de seuil qui définissent trois plages de valeurs de données (basse, moyenne et haute) à laquelle vous pouvez appliquer une couleur différente (ou un style différent).</span><span class="sxs-lookup"><span data-stu-id="29e7d-108">To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different color (or style).</span></span>

## <a name="to-set-up-colored-indicators-on-cues"></a><span data-ttu-id="29e7d-109">Pour paramétrer des indicateurs colorés sur des piles</span><span class="sxs-lookup"><span data-stu-id="29e7d-109">To set up colored indicators on Cues</span></span>
1. <span data-ttu-id="29e7d-110">Sous **Activités** sur votre page **Accueil**, sélectionnez **Paramétrer piles**.</span><span class="sxs-lookup"><span data-stu-id="29e7d-110">Under **Activities** on your **Home** page, choose **Set Up Cues**.</span></span>  
<span data-ttu-id="29e7d-111">La fenêtre **Paramètres pile** s'affiche.</span><span class="sxs-lookup"><span data-stu-id="29e7d-111">The **Cue Setup** window appears.</span></span> <span data-ttu-id="29e7d-112">La fenêtre répertorie les indicateurs actuellement paramétrés sur des piles.</span><span class="sxs-lookup"><span data-stu-id="29e7d-112">The window lists the indicators that are currently setup up on Cues.</span></span>
2. <span data-ttu-id="29e7d-113">Pour modifier un indicateur, modifiez les champs et modifiez, par exemple, les valeurs pour des seuils différents.</span><span class="sxs-lookup"><span data-stu-id="29e7d-113">To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.</span></span>  

<span data-ttu-id="29e7d-114">Le tableau suivant répertorie les couleurs correspondant aux options des champs **Style bas de gamme**, **Style milieu de gamme** et **Style haut de gamme**.</span><span class="sxs-lookup"><span data-stu-id="29e7d-114">The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.</span></span>

|<span data-ttu-id="29e7d-115">Option</span><span class="sxs-lookup"><span data-stu-id="29e7d-115">Option</span></span>|<span data-ttu-id="29e7d-116">Couleur</span><span class="sxs-lookup"><span data-stu-id="29e7d-116">Color</span></span>|
|------|-----|
|<span data-ttu-id="29e7d-117">**Aucun**</span><span class="sxs-lookup"><span data-stu-id="29e7d-117">**None**</span></span>|<span data-ttu-id="29e7d-118">Aucune couleur (même couleur que la mosaïque Pile</span><span class="sxs-lookup"><span data-stu-id="29e7d-118">No color (same color as the Cue tile</span></span>|
|<span data-ttu-id="29e7d-119">**Favorable**</span><span class="sxs-lookup"><span data-stu-id="29e7d-119">**Favorable**</span></span>|<span data-ttu-id="29e7d-120">Vert</span><span class="sxs-lookup"><span data-stu-id="29e7d-120">Green</span></span>|
|<span data-ttu-id="29e7d-121">**Défavorable**</span><span class="sxs-lookup"><span data-stu-id="29e7d-121">**Unfavorable**</span></span>|<span data-ttu-id="29e7d-122">Rouge</span><span class="sxs-lookup"><span data-stu-id="29e7d-122">Red</span></span>|
|<span data-ttu-id="29e7d-123">**Ambigu**</span><span class="sxs-lookup"><span data-stu-id="29e7d-123">**Ambiguous**</span></span>|<span data-ttu-id="29e7d-124">Jaune</span><span class="sxs-lookup"><span data-stu-id="29e7d-124">Yellow</span></span>|
|<span data-ttu-id="29e7d-125">**Subordonné**</span><span class="sxs-lookup"><span data-stu-id="29e7d-125">**Subordinate**</span></span>|<span data-ttu-id="29e7d-126">Gris</span><span class="sxs-lookup"><span data-stu-id="29e7d-126">Gray</span></span>|

## <a name="see-also"></a><span data-ttu-id="29e7d-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="29e7d-127">See Also</span></span>
[<span data-ttu-id="29e7d-128">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="29e7d-128">Work with Dynamics NAV</span></span>](ui-work-product.md)


