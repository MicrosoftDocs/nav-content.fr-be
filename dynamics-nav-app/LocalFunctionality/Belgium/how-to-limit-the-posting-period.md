---
title: "Comment limiter la période de validation"
description: "Vous pouvez limiter la période au cours de laquelle la validation est autorisée selon trois niveaux différents : **par société**, **par utilisateur** et **par modèle**."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 0fd8eca40a1b057458dac369931f7f4a39c832d4
ms.contentlocale: fr-be
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-limit-the-posting-period"></a>Comment limiter la période de validation
Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez limiter la période au cours de laquelle la validation est autorisée selon trois niveaux différents : **par société**, **par utilisateur** et **par modèle**.  

Il peut être utile de limiter les périodes de validation lorsqu'une société clôture sa feuille vente à la fin de chaque mois. Cela empêche les vendeurs d'enregistrer des documents vente du mois précédent. Dans le même temps, la feuille achat peut rester ouverte pour enregistrer les factures achat entrantes du mois précédent.  

Lorsque vous effectuez une validation dans la fenêtre **Modèles feuille comptabilité**, le contenu des champs **Début période validation** et **Fin période validation** est vérifié pour obtenir un intervalle de dates. L'intervalle de date indique à quel moment vous pouvez valider sur un modèle feuille. Si le champ est vide, la fenêtre **Paramètres utilisateur** est vérifiée pour obtenir un intervalle de dates pour l'utilisateur actuel. Si la fenêtre **Paramètres utilisateur** ne contient pas d'intervalle, les champs **Début période validation** et **Fin période validation** dans la fenêtre **Paramètres comptabilité** sont vérifiés pour obtenir un intervalle de dates au niveau de la société.  

## <a name="to-limit-the-posting-periods-by-company"></a>Pour limiter les périodes de validation par société  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Paramètres comptabilité**, puis sélectionnez le lien correspondant.  
2.  Pour spécifier le début de la période, choisissez le champ **Début période validation**, puis entrez la première date à laquelle la validation sur la société est autorisée.  
3.  Pour spécifier la fin de la période, choisissez le champ **Fin période validation**, puis entrez la dernière date à laquelle la validation sur la société est autorisée.  

## <a name="to-limit-the-posting-periods-by-user"></a>Pour limiter les périodes de validation par utilisateur  

1.  Choisissiez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres utilisateur**, puis sélectionnez le lien correspondant.  
2.  Pour spécifier le début de la période, choisissez le champ **Début période validation**, puis entrez la première date à laquelle l'utilisateur peut effectuer la validation sur la société.  
3.  Pour spécifier la fin de la période, choisissez le champ **Fin période validation**, puis entrez la dernière date à laquelle l'utilisateur peut effectuer la validation sur la société.  

## <a name="to-limit-the-posting-periods-by-template"></a>Pour limiter les périodes de validation par modèle  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Modèles feuille comptabilité**, puis sélectionnez le lien correspondant.  
2.  Pour spécifier le début de la période, choisissez le champ **Début période validation**, puis entrez la première date à laquelle l'utilisateur peut effectuer la validation sur la société.  
3.  Pour spécifier la fin de la période, choisissez le champ **Fin période validation**, puis entrez la dernière date à laquelle l'utilisateur peut effectuer la validation sur la société.  

## <a name="see-also"></a>Voir aussi  
 [Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)   
 [Comment spécifier des périodes de validation](../../finance-how-specify-posting-periods.md)

