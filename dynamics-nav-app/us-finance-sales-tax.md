---
title: "Taxe sur les ventes et groupes de taxes aux États-Unis et au Canada"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f70a191fc8392bf1685c08c7e905ac96ba7ed069
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-tax-groups-in-the-us-and-canada"></a>Taxe sur les ventes et groupes de taxes aux États-Unis et au Canada
Lorsque vous commencez à utiliser Dynamics NAV, vous pouvez exécuter un guide de configuration assistée afin de rapidement et facilement configurer les informations relatives à la Sales Tax pour votre société et éventuellement pour vos clients et vos fournisseurs. En quelques minutes, vous êtes prêt à créer des documents vente et des documents achat pour lesquels la Sales Tax est calculée correctement.
Si vous passez à la section Ma société vierge, nous vous recommandons de commencer par utiliser chacun des guides de configuration assistée, y compris celui qui concerne la Sales Tax. Si vous préférez configurer la Sales Tax par vous-même, cet article explique ce que vous devez prendre en compte.  

## <a name="tax-groups-tax-areas-and-tax-jurisdictions"></a>Groupes taxes, zones de recouvrement et autorités de recouvrement
Dans Dynamics NAV, un groupe taxes représente un groupe d'articles en stock ou de ressources soumis aux mêmes conditions fiscales. Par exemple, vous pouvez configurer un groupe taxes pour les articles soumis à la taxe et un autre pour les articles non soumis à la taxe. Vous devez affecter des codes groupe taxes aux articles en stock et aux comptes généraux. De même, vous devez affecter des codes zone recouvrement aux clients, aux magasins et à vos propres paramètres de société. Le guide de configuration assistée vous aide à effectuer ces opérations.  

Chaque zone recouvrement correspond à un regroupement d'autorités fiscales basé sur une situation géographique particulière. Par exemple, la zone recouvrement de Miami, Floride, comprend trois autorités fiscales de la Sales Tax : la ville (Miami), le comté (Dade) et l'état (Floride). Dynamics NAV inclut un ensemble limité de zones de recouvrement avec une configuration par défaut, mais vous pouvez les modifier et ajouter de nouvelles zones de recouvrement.  

Si vous configurez de nouvelles zones et juridictions de recouvrement, vous devez veiller à bien remplir les champs correctement. Aux États-Unis, les états, les régions, les villes et les localités peuvent prélever la taxe sur les ventes. Au Canada, le gouvernemental fédéral et les provinces sont en mesure de prélever la Sales Tax. Les sociétés recueillent et la Sales Tax et la versent aux autorités gouvernementales pour les produits vendus aux utilisateurs finaux. La Sales Tax peut également être facturée sur une Sales Tax existante. Par exemple, la taxe peut être calculée sur un montant facture vente qui comprend déjà la taxe imposée par d'autres autorités.  

Au Canada, les montants de taxe doivent être détaillés dans les documents concernant chaque autorité de recouvrement. Jusqu'à quatre autorités de recouvrement peuvent apparaître dans un document, et les autorités dotées du même ordre d'impression sont regroupées lors de l'impression.

## <a name="tax-details"></a>USA spécifications taxe
La fenêtre **USA spécifications taxe** affiche différentes combinaisons de zones de recouvrement de la Sales Tax et de groupes de taxe afin d'établir les taux de taxe. Pour chaque autorité de recouvrement, nous vous recommandons de configurer un groupe taxes pour la Sales Tax normale, un autre groupe taxes pour les articles ou les services qui ne sont pas soumis à la taxe et un groupe taxes supplémentaire pour chaque type d'article ou de service traité avec un taux de taxe différent dans cette zone de recouvrement.  

Aux États-Unis, lorsque vous vendez à un client dans un magasin où vous n'avez pas de *situs*(ou un magasin légal dans cet état) vous ne percevez pas la Sales Tax. Pour les magasins dans lesquels vous n'avez pas de situs, assurez-vous que la valeur des champs **Taxe inférieure minimum** and **Taxe supérieure maximum** est égale à 0,00.  

## <a name="see-also"></a>Voir aussi
[Finance](finance-setup.md)  
[Configuration de la finance](finance-setup-setup-finance-setup.md)  
[Taxe sur les ventes et taxe sur les biens et les services au Canada](ca-finance-setup-tax.md)  
[Configuration simplifiée de la Sales Tax](https://madeira.microsoft.com/en-us/blog/sales-tax-setup-made-easy)  

