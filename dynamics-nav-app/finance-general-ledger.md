---
title: "Les écritures comptables et le plan comptable"
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
ms.openlocfilehash: 9965ddcad214e97c5e4858824395d6f651b3c003
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="the-general-ledger-and-the-chart-of-accounts"></a>Les écritures comptables et le plan comptable
Les écritures comptables stockent vos données financières, et le plan comptable affiche les comptes sur lesquels toutes les écritures comptables sont validées. Dynamics NAV inclut un plan comptable standard prêt à prendre en charge votre société.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Configuration des écritures comptable et configuration de la comptabilisation
Les écritures comptables sont à la base de vos processus entreprise, ainsi que la configuration de la manière dont les données y sont validées.
Dans la fenêtre **Paramètres comptabilité**, vous spécifiez comment gérer certains problèmes comptables dans votre société. Ceci inclut les détails arrondi facture, les formats d'adresse, et si vous souhaitez utiliser une devise report supplémentaire, par exemple.
De même, dans la fenêtre **Paramètres comptabilisation**, vous spécifiez comment vous souhaitez configurer les combinaisons de groupes généraux comptabilisation marché et de groupes généraux comptabilisation produit. Saisissez une ligne pour chaque combinaison de groupes comptabilisation marché et de groupes comptabilisation produit.  

## <a name="the-chart-of-accounts"></a>Le plan comptable
Le plan comptable affiche tous les comptes. Depuis cette fenêtre, vous pouvez ouvrir divers états qui affichent vos écritures comptables et vos soldes, et vous pouvez clôturer le compte de gestion. Pour chaque compte, vous pouvez ouvrir la fiche compte général et ajouter ou modifier les paramètres. Vous pouvez également afficher la liste des groupes comptabilisation qui effectuent les validations vers ce compte.  

Dynamics NAV vous empêchera de supprimer un compte général qui stocke les données nécessaires au plan comptable.  

## <a name="account-categories"></a>Catégories de compte
Avec les catégories de compte, vous pouvez associer les comptes généraux à des catégories afin de personnaliser la structure de vos états financiers.  

La fenêtre **Catégories de compte général** affiche vos catégories et sous-catégories principales existantes et les comptes généraux que vous avez affecté à chaque catégorie. Vous pouvez créer des sous-catégories et affecter ces catégories à des comptes existants.  

Vous pouvez regrouper les catégories de compte en effectuant une indentation des sous-catégories individuelles. Cela vous facilite l'obtention d'une vue d'ensemble, car chaque groupement affiche un solde final. Par exemple, vous pouvez créer des sous-catégories pour différents types d'actifs puis créer des groupes des catégories pour différencier les immobilisations des actifs à court terme, par exemple. Vous créez un groupe des catégories en effectuant une indentation d'autres sous-catégories sous une ligne de la fenêtre **Catégories de compte général**.  

Pour chaque sous-catégorie, vous pouvez spécifier si les comptes de cette catégorie doivent être inclus dans des types spécifiques d'états financiers. Les catégories de compte vous aident à définir la présentation de vos états financiers. Par exemple, le solde relevé par défaut solde est doté d'une seule écriture pour la trésorerie dans les actifs. Si vous souhaitez que le solde relevé soit doté de sous-entrées pour le fonds de caisse et votre compte chèque, vous pouvez ajouter deux nouvelles sous-catégories, spécifier la définition d'état supplémentaire Comptes de trésorerie pour chacun d'eux, et effectuer une indentation sous la sous-catégorie Trésorerie. Ensuite, lorsque vous avez généré les tableaux d'analyse en fonction de vos modifications, votre relevé solde suivant affichera un solde final pour la trésorerie et deux lignes avec les soldes pour le fonds de caisse et le compte chèque.     

##<a name="see-also"></a>Voir aussi
[Finance](finance-setup.md)  
[Configuration ou modification du plan comptable](finance-setup-setup-chart-accounts.md)  
[Tableaux d'analyse](finance-setup-account-schedule.md)  

