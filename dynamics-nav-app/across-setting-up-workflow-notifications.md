---
title: Configuration de notifications de flux de travail
description: "Pour un grand nombre de réponses de workflow, il s'agit de notifier un utilisateur qu'un événement s'est produit et qu'il doit agir dessus. Par exemple, dans une étape du workflow, l'événement peut être que l'utilisateur 1 demande l'approbation d'un nouvel enregistrement, et la réponse est qu'une notification est envoyée à l'utilisateur 2, l'approbateur. Dans l'étape suivante du workflow, l'événement peut être que l'utilisateur 2 approuve l'enregistrement, et la réponse est qu'une notification est envoyée à l'utilisateur 3 pour qu'il démarre le processus associé à l'enregistrement approuvé. Pour les étapes de flux de travail concernant des approbations, chaque notification est liée à une écriture d'approbation."
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
ms.openlocfilehash: 2c3e64a5d343bad026ba5417f18861ef6417dae3
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-workflow-notifications"></a><span data-ttu-id="e9d5d-106">Configuration de notifications de flux de travail</span><span class="sxs-lookup"><span data-stu-id="e9d5d-106">Setting Up Workflow Notifications</span></span>
<span data-ttu-id="e9d5d-107">Pour un grand nombre de réponses de workflow, il s'agit de notifier un utilisateur qu'un événement s'est produit et qu'il doit agir dessus.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-107">Many workflow responses are about notifying a user that an event has occurred that they must act on.</span></span> <span data-ttu-id="e9d5d-108">Par exemple, dans une étape du workflow, l'événement peut être que l'utilisateur 1 demande l'approbation d'un nouvel enregistrement, et la réponse est qu'une notification est envoyée à l'utilisateur 2, l'approbateur.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-108">For example, on one workflow step, the event can be that User 1 requests approval of a new record, and the response is that a notification is sent to User 2, the approver.</span></span> <span data-ttu-id="e9d5d-109">Dans l'étape suivante du workflow, l'événement peut être que l'utilisateur 2 approuve l'enregistrement, et la réponse est qu'une notification est envoyée à l'utilisateur 3 pour qu'il démarre le processus associé à l'enregistrement approuvé.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-109">On the next workflow step, the event can be that User 2 approves the record, and the response is that a notification is sent to User 3 to start a related processing of the approved record.</span></span> <span data-ttu-id="e9d5d-110">Pour les étapes de flux de travail concernant des approbations, chaque notification est liée à une écriture d'approbation.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-110">For workflow steps that are about approval, each notification is tied to an approval entry.</span></span> <span data-ttu-id="e9d5d-111">Pour plus d'informations, voir [Flux de travail](across-workflow.md).</span><span class="sxs-lookup"><span data-stu-id="e9d5d-111">For more information, see [Workflow](across-workflow.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="e9d5d-112">La version générique de [!INCLUDE[d365fin](includes/d365fin_md.md)] prend en charge des notifications comme des e\-mails et des notes internes.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] supports notifications as email and as internal notes.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="e9d5d-113">Toutes les notifications du workflow sont envoyées à l'aide d'une file projets.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-113">All workflow notifications are sent through a job queue.</span></span> <span data-ttu-id="e9d5d-114">Assurez-vous que la file projets figure dans votre solution.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-114">Make sure that the job queue in your solution.</span></span> <span data-ttu-id="e9d5d-115">Pour plus d'informations, voir [Utiliser des files d'attente des travaux pour planifier des tâches](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="e9d5d-115">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

<span data-ttu-id="e9d5d-116">Vous pouvez configurer différents aspects des notifications du workflow dans les emplacements suivants :</span><span class="sxs-lookup"><span data-stu-id="e9d5d-116">You set up different aspects of workflow notifications in the following places:</span></span>  

1.  <span data-ttu-id="e9d5d-117">Pour des workflows d'approbation, configurez les destinataires des notifications du workflow en renseignant une ligne dans la fenêtre **Paramètres utilisateur approbation** pour chaque utilisateur qui fait partie du workflow.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-117">For approval workflows, you set up the recipients of workflow notifications by filling a line in the **Approval User Setup** window for each user that takes part in the workflow.</span></span> <span data-ttu-id="e9d5d-118">Par exemple, si l'utilisateur 2 est spécifié dans le champ **ID Approbateur** sur la ligne de l'utilisateur 1, alors la notification de demande d'approbation est envoyée à l'utilisateur 1.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-118">For example, if User 2 is specified in the **Approver ID** field on the line for User 1, then the approval request notification is sent to User 1.</span></span> <span data-ttu-id="e9d5d-119">Pour plus d'informations, voir [Procédure : configurer des utilisateurs d'approbation](across-how-to-set-up-approval-users.md).</span><span class="sxs-lookup"><span data-stu-id="e9d5d-119">For more information, see [How to: Set Up Approval Users](across-how-to-set-up-approval-users.md).</span></span>  
2.  <span data-ttu-id="e9d5d-120">Vous définissez quand et comment les utilisateurs reçoivent des notifications de workflow en renseignant la fenêtre **Tableau de notification** pour chaque utilisateur du workflow.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-120">You set when and how users receive workflow notifications by filling the **Notification Schedule** window for each workflow user.</span></span> <span data-ttu-id="e9d5d-121">Pour plus d'informations, voir [Procédure : spécifier quand et comment recevoir des notifications](across-how-to-specify-when-and-how-to-receive-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="e9d5d-121">For more information, see [How to: Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md).</span></span>  
3.  <span data-ttu-id="e9d5d-122">Vous configurez le contenu général et la mise en forme des notifications, y compris les notifications concernant les réponses de workflow échues, en configurant des modèles de notification dans la fenêtre **Modèles de notification**.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-122">You set up the general content and layout of notifications, including notifications about overdue workflow responses, by setting up notification templates in the **Notification Templates** window.</span></span> <span data-ttu-id="e9d5d-123">Vous pouvez utiliser les modèles par défaut fournis avec [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e9d5d-123">You can use the default templates provided with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
4.  <span data-ttu-id="e9d5d-124">Vous configurez un contenu spécifique et des règles d'une notification de workflow lorsque vous créez le workflow en question.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-124">You set up specific content and rules of a workflow notification when you create the workflow in question.</span></span> <span data-ttu-id="e9d5d-125">Pour effectuer cette opération, sélectionnez les options dans la fenêtre **Options réponse de flux de travail** pour la réponse de workflow qui représente la notification.</span><span class="sxs-lookup"><span data-stu-id="e9d5d-125">You do this by selecting options in the **Workflow Response Options** window for the workflow response that represents the notification.</span></span> <span data-ttu-id="e9d5d-126">Pour plus d'informations, reportez-vous à l'étape 9 dans [Procédure : créer des workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="e9d5d-126">For more information, see step 9 in [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="e9d5d-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e9d5d-127">See Also</span></span>  
 <span data-ttu-id="e9d5d-128">[Procédure : configurer des utilisateurs d'approbation](across-how-to-set-up-approval-users.md) </span><span class="sxs-lookup"><span data-stu-id="e9d5d-128">[How to: Set Up Approval Users](across-how-to-set-up-approval-users.md) </span></span>  
 <span data-ttu-id="e9d5d-129">[Procédure : configurer des utilisateurs de workflow](across-how-to-set-up-workflow-users.md) </span><span class="sxs-lookup"><span data-stu-id="e9d5d-129">[How to: Set Up Workflow Users](across-how-to-set-up-workflow-users.md) </span></span>  
 <span data-ttu-id="e9d5d-130">[Procédure : spécifier quand et comment recevoir des notifications](across-how-to-specify-when-and-how-to-receive-notifications.md) </span><span class="sxs-lookup"><span data-stu-id="e9d5d-130">[How to: Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md) </span></span>  
 <span data-ttu-id="e9d5d-131">[Procédure : créer des workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="e9d5d-131">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="e9d5d-132">[Procédure : gérer les modèles de notification](across-how-to-manage-notification-templates.md) </span><span class="sxs-lookup"><span data-stu-id="e9d5d-132">[How to: Manage Notification Templates](across-how-to-manage-notification-templates.md) </span></span>  
 <span data-ttu-id="e9d5d-133">[Utiliser des files d'attente des travaux pour planifier des tâches](admin-job-queues-schedule-tasks.md) </span><span class="sxs-lookup"><span data-stu-id="e9d5d-133">[Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md) </span></span>  
 <span data-ttu-id="e9d5d-134">[Procédure : configurer la messagerie](madeira-how-setup-email.md) </span><span class="sxs-lookup"><span data-stu-id="e9d5d-134">[How to: Set up Email](madeira-how-setup-email.md) </span></span>  
 <span data-ttu-id="e9d5d-135">[Procédure pas à pas : Configuration et utilisation d'un flux d'approbation achat](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="e9d5d-135">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 [<span data-ttu-id="e9d5d-136">Flux de travail</span><span class="sxs-lookup"><span data-stu-id="e9d5d-136">Workflow</span></span>](across-workflow.md)   
