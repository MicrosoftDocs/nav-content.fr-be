---
title: "Paramétrer les statuts des commandes service et des réparations"
description: "Vous devez paramétrer neuf états réparation qui identifient la progression de la réparation et de la maintenance des articles de service des commandes service."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d7dbc4cfc06d4c74476a04512bd368a0ab26f837
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-statuses-for-service-orders-and-repairs"></a>Procédure : paramétrer les statuts des commandes service et des réparations
Vous devez paramétrer des états réparation qui identifient la progression de la réparation et de la maintenance des articles de service des commandes service. Vous devez configurer au moins neuf options de statut réparation identifiant les situations ou les actions effectuées lors de la maintenance des articles de service.  

Vous pouvez définir le niveau de priorité des options de statut commande service. Quatre niveaux de priorité sont disponibles : Très haute, Haute, Moyenne et Basse.  
  
Lorsque vous modifiez le statut réparation d'un article de service d'une commande service, le statut commande service est mis à jour. Le statut réparation de chaque article de service est lié au statut commande service. Si les articles de service sont liés à plusieurs options de statut commande service, le statut de commande service dont la priorité est la plus élevée est sélectionnée.  

## <a name="to-set-up-a-repair-status"></a>Pour configurer le statut réparation  
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Etat de la réparation**, puis sélectionnez le lien connexe. 2. Créez un état réparation.  
3. Renseignez les champs **Code** et **Désignation**.  
4. Dans le champ **Statut commande service**, choisissez le statut de la commande auquel lier l'état de réparation. Le champ **Priorité** affiche la priorité du statut commande service que vous avez choisie.  
5. Choisissez un état réparation. Vous ne pouvez en choisir qu'un.  
6. Pour valider des commandes service comprenant des articles de service avec cet état réparation, choisissez le champ **Validation autorisée**.  
7. Pour pouvoir faire passer manuellement l'option de statut commande service sur **Suspendu** dans des commandes service comprenant des articles de service avec ce statut réparation, choisissez la case à cocher **Statut Suspendu autorisé**.  
8. Choisissez de la même manière les cases à cocher **Statut En cours autorisé**, **Statut Terminé autorisé** et **Statut En attente autorisé**.
  
## <a name="to-set-up-service-status-priorities"></a>Pour configurer les priorités statut service  
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Statut commande service**, puis sélectionnez le lien connexe.  
2. Sélectionnez le statut commande service pour lequel vous voulez configurer une priorité.  
3. Dans le champ **Priorité**, choisissez la priorité souhaitée pour ce statut commande service. Répétez cette étape pour chaque statut.  
  
## <a name="see-also"></a>Voir aussi  
[Description des commandes service et de l'état réparation]()  
[Paramétrage de la gestion des services](service-setup-service.md)  

