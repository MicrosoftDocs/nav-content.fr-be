---
title: "Procédure : configurer les centres de charge et les postes de charge"
description: "Les fiches **Centre de charge** organisent les exigences et les valeurs fixes des ressources de production, et régissent ainsi la production des centres de charge."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/19/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: ba71815bc7d099b7f600ab828dec579ddbf2265a
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-work-centers-and-machine-centers"></a>Procédure : configurer les centres de charge et les postes de charge
L'application distingue trois types de capacité. Ces capacités sont ordonnées de façon hiérarchique. Chaque niveau contient les niveaux subordonnés.  

Le premier niveau correspond au groupe centres de charge. Des centres de charge sont affectés aux groupes centres de charge. Chaque centre de charge ne peut appartenir qu'à un seul groupe centres de charge.

Vous pouvez affecter plusieurs postes de charge à chaque centre de charge. Un poste de charge ne peut appartenir qu'à un seul centre de charge.  

La capacité planifiée d'un centre de charge se compose de la disponibilité des postes de charge correspondants et de la disponibilité planifiée du centre de charge. La disponibilité planifiée du groupe centres de charge correspond donc au total de toutes les disponibilités des postes de charge et des centres de charge qui le composent.  

La disponibilité est enregistrée dans les écritures calendrier. Avant de configurer des centres ou postes de charge, vous devez configurer des calendriers usine. Pour plus d'informations, voir [Procédure : créer des calendriers usine](production-how-to-create-work-center-calendars.md).  

## <a name="to-set-up-a-work-center"></a>Pour configurer un centre de charge
La procédure suivante décrit essentiellement comment configurer un centre de charge. La procédure de configuration d'un calendrier poste de charge est similaire, sauf pour le raccourci **Paramètres gamme**.  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Centres de charge**, puis sélectionnez le lien connexe.  
2.  Sélectionnez l'action **Nouveau**.  
3. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Dans le champ **Groupe centres de charge**, sélectionnez le regroupement de ressources de niveau supérieur sous lequel le centre de charge est organisé, au besoin. Choisissez l'action **Nouveau** dans la liste déroulante.  
5.  Sélectionnez le champ **Bloqué** pour empêcher le centre de charge d'être utilisé pour quelque traitement que ce soit. Cela signifie que la production ne peut pas être validée pour un article produit dans le centre de charge. Pour plus d'informations, voir [Procédure : valider la production](production-how-to-post-output-quantity.md).
6.  Dans le champ **Coût unitaire direct**, entrez le coût de production d'une unité de mesure dans le centre de charge, sans intégrer les autres éléments de coût. Ce coût est souvent appelé *frais de main-d'œuvre directs*.  
7.  Dans le champ **% coût indirect**, entrez les coûts opératoires généraux de l'utilisation du centre de charge sous la forme d'un pourcentage du coût unitaire direct. Ce pourcentage est ajouté au coût direct lors du calcul du coût unitaire.  
8.  Dans le champ **Frais généraux**, entrez tous les coûts non opératoires, comme les frais de maintenance, du centre de charge sous la forme d'un montant absolu.  

    Le champ **Coût unitaire** affiche le résultat du calcul du coût unitaire de production d'une unité de mesure dans le centre de charge. Tous les éléments de coût sont pris en compte comme suit :  

    Coût unitaire = Coût unitaire direct + (Coût unitaire direct x % coût indirect) + Frais généraux.  

9.  Dans le champ **Unité de coût**, indiquez si le calcul ci-dessus doit être basé sur le délai passé : **Heure** ou sur le nombre d'unités produites : **Unités**.  
10.  Sélectionnez le champ **Coût unitaire spécifique** pour définir le coût unitaire du centre de charge sur la ligne gamme dans laquelle il est utilisé. Ceci peut s'avérer utile pour les opérations dont les coûts opératoires diffèrent radicalement de ceux normalement traités dans le centre de charge.  
11.  Dans le champ **Méthode consommation**, indiquez si la validation de production du centre de charge doit être calculée et validée manuellement ou automatiquement, de l'une des manières suivantes.  

    |Option|Désignation|  
    |----------------------------------|---------------------------------------|  
    |**Manuel**|La consommation est validée manuellement dans la feuille production.|
    |**Aval**|La consommation est calculée et validée automatiquement lorsque l'ordre de fabrication est émis.|  
    |**Amont**|La consommation est calculée et validée automatiquement lorsque l'ordre de fabrication est terminé.|  

    > [!NOTE]  
    >  Si nécessaire, vous pouvez modifier la méthode de consommation sélectionnée ici et sur la fiche **article** pour des opérations précises en modifiant le paramétrage des lignes gamme.

12.  Dans le champ **Code unité**, entrez l'unité de temps utilisée pour le calcul de coût et la planification de capacité du centre de charge.
    Pour contrôler en permanence la consommation, vous devez d'abord définir une méthode de mesure. Les unités que vous saisissez sont des unités de base. Par exemple, la durée de traitement est mesurée en heures et en minutes.

    > [!NOTE]  
    > Si vous choisissez d'utiliser Jours, n'oubliez pas qu'1 jour = 24 heures et non 8 (heures de travail).

13.  Dans le champ **Capacité**, indiquez si le centre de charge a plusieurs postes ou personnes travaillant simultanément. Si votre installation de [!INCLUDE[d365fin](includes/d365fin_md.md)] n'inclut pas la fonctionnalité de poste de charge, la valeur de ce champ doit être **1**.  
14.  Dans le champ **Rendement**, entrez le pourcentage de la production standard prévue qui est réalisé par le centre de charge. Si vous entrez **100**, cela signifie que la production réelle du centre de charge est identique à la production standard.  
15. Activez la case à cocher **Calendrier consolidé** si vous utilisez également des postes de charge. Ainsi, les écritures calendrier sont générées à partir des calendriers de poste de charge.  
16.  Dans le champ **Code calendrier usine**, sélectionnez un calendrier usine. Pour plus d'informations, voir [Procédure : créer des calendriers usine](production-how-to-create-work-center-calendars.md).  
17.  Dans le champ **File d'attente**, spécifiez le délai fixe qui doit s'écouler avant que le travail attribué ne commence dans le centre de charge. Notez que la file d'attente ainsi définie est ajoutée aux autres éléments de temps non productifs, tels que le temps d'attente et le temps de transfert, définis sur les lignes gamme utilisant ce centre de charge.  

## <a name="example---different-machine-centers-assigned-to-a-work-center"></a>Exemple - Plusieurs postes de charge sont affectés à un centre de charge
Lors de la configuration des postes et des centres de charge, il convient de planifier les capacités constituant la capacité totale.

Si différents postes de charge (tels que 210 Table d'emballage 1, 310 Cabine de peinture...) sont affectés à un centre de charge, il convient de prendre en compte les capacités de chaque poste de charge, car la panne de l'un de ces postes risque d'interrompre l'ensemble du processus. Vous pouvez saisir les groupes postes en fonction de leur capacité mais vous ne pouvez pas les inclure dans le planning. Lorsque vous désactivez le champ **Calendrier consolidé**, seule la capacité du centre de charge est affectée au planning, pas le poste de charge.

Toutefois, lorsqu'un centre de charge combine des postes de charge identiques (tels que 210 Table d'emballage 1 et 220 Table d'emballage 2), il convient de prendre en compte ce centre de charge en tant que somme des postes de charge affectés. Le centre de charge est donc répertorié avec une capacité zéro. La capacité commune est affectée au centre de charge lorsque vous activez le champ **Calendrier consolidé**.

Lorsque les capacités des centres de charge n'ajoutent en rien à la capacité totale, vous pouvez paramétrer Rendement = 0.

## <a name="to-set-up-a-capacity-constrained-machine-or-work-center"></a>Pour configurer un centre de charge ou un poste de charge à la capacité critique
Vous devez configurer les ressources de production que vous considérez comme critique et de l'accepter comme une charge limitée au lieu de la charge illimitée par défaut que d'autres ressources de production acceptent. Une capacité critique peut être un centre de charge ou un poste de charge que vous avez identifié comme étant un goulot d'étranglement et pour lequel vous souhaitez établir une charge limitée.

[!INCLUDE[d365fin](includes/d365fin_md.md)] ne prend pas en charge le contrôle détaillé d'atelier. Il prévoit une utilisation des ressources faisable via une planification approximative, mais il ne crée ni ne met à jour automatiquement des plannings détaillés sur la base des priorités ou des règles d'optimisation.

Dans la fenêtre **Capacités critiques**, vous pouvez effectuer un paramétrage qui évite la surcharge de ressources spécifiques et permet de s'assurer qu'aucune capacité n'est laissée non affectée si elle peut augmenter le délai d'exécution d'un ordre de fabrication. Dans le champ **Seuil (% capacité totale)**, vous pouvez ajouter un seuil aux ressources afin de réduire la répartition des opérations. Cela permet au système de planifier la charge sur le dernier jour possible en dépassant légèrement le pourcentage de charge critique si ceci peut réduire le nombre d'opérations qui sont divisées.

Lors de la planification avec des ressources avec contraintes de capacité, le système veille à ce qu'aucune ressource ne soit chargée au-dessus de sa capacité définie (charge critique). Ceci est effectué en affectant chaque opération à l'emplacement du temps disponible le plus proche. Si le créneau n'est pas assez long pour effectuer toute l'opération, l'opération est répartie en au moins deux parties placées dans les créneaux disponibles les plus proches.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Capacités critiques**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau**.
3. Renseignez les champs selon vos besoins.

> [!NOTE]
> Les opérations de postes ou de centres de charge qui sont configurées comme ressources contraintes sont toujours planifiées en série. Cela signifie que même si une ressource contrainte a plusieurs capacités, ces capacités ne peuvent être planifiées que dans l'ordre, pas en parallèle, comme c'est le cas si le poste ou le centre de charge n'a pas été défini en tant que ressource contrainte. Dans une ressource contrainte, le champ Capacité du centre ou du poste de charge est supérieur à 1.

> En cas de répartition des opérations, le temps de préparation n'est affecté qu'une fois car on suppose qu'un certain ajustement manuel est effectué pour optimiser le planning.

## <a name="see-also"></a>Voir aussi  
[Procédure : créer des calendriers usine](production-how-to-create-work-center-calendars.md)  
[Paramétrage de la production](production-configure-production-processes.md)  
[Production](production-manage-manufacturing.md)    
[Planifié](production-planning.md)   
[STOCKS ET EN-COURS](inventory-manage-inventory.md)  
[Achats](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

