---
title: "Paramétrer la maintenance des immobilisations"
description: "Pour gérer les réparations et la maintenance des immobilisations, spécifiez les informations de maintenance générale, les codes du type de travail, et un compte de validation pour les coûts."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: repair, service
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cb437985793e7fa4330d5bd8301d2808b5deafcc
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-fixed-asset-maintenance"></a>Procédure : configurer une maintenance d'immobilisation
Pour gérer la maintenance des immobilisations, vous devez configurer tout d'abord certaines informations générales de maintenance, un compte de validation pour les coûts de maintenance et les codes de maintenance pour les types de travaux, tels que le service de routine ou la réparation.

## <a name="to-set-up-general-maintenance-information"></a>Pour configurer les informations générales de maintenance
Si vous configurez les champs pour la maintenance, vous pouvez valider des frais de maintenance à partir d'une feuille immobilisation.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Immobilisations**, puis sélectionnez le lien connexe.
2. Sélectionnez l'immobilisation pour laquelle vous souhaitez définir la couverture d'assurance, puis sélectionnez l'action **Modifier**.
3. Sur le raccourci **Maintenance**, complétez les champs, comme nécessaire. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-maintenance-codes"></a>Pour configurer des codes maintenance
Lorsque vous validez des coûts de maintenance à partir d'une feuille comptabilité, vous renseignez le champ **Code maintenance** pour enregistrer le type de maintenance effectuée, telle qu'un service de routine ou une réparation.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Maintenance**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Maintenance**, configurez les codes pour les différents types de travaux de maintenance.

## <a name="to-set-up-maintenance-expense-accounts"></a>Pour configurer des comptes frais de maintenance
Pour valider les coûts de maintenance, vous devez tout d'abord saisir un numéro de compte dans la fenêtre **Groupes compta. immo**.

1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Groupes compta. immo.**, puis choisissez le lien associé.
2. Renseignez le champ **Compte frais maintenance** pour chaque groupe comptabilisation.

> [!NOTE]  
>   Pour définir que les coûts de maintenance sont attribués aux départements ou projets, configurez une clé d'allocation. Pour en savoir plus, voir [Procédure : configurer des fonctionnalités d'immobilisations](fa-how-setup-general.md).

## <a name="see-also"></a>Voir aussi
[Paramétrage d'immobilisations](fa-setup.md)  
[Immobilisations](fa-manage.md)  
[Finances](finance.md)  
[Bienvenue dans [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

