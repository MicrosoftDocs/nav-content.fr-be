---
title: Configuration ou modification du plan comptable
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 48cd91958545b40b2ab0c5e48442fc874845af5b
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a>Configuration ou modification du plan comptable
Le plan comptable affiche les comptes généraux qui stockent vos données financières. Dynamics NAV inclut un plan comptable standard prêt à prendre en charge votre société.
Cependant, vous pouvez modifier les comptes par défaut, et vous pouvez ajouter de nouveaux comptes.  

## <a name="adding-or-changing-accounts"></a>Ajout ou modification de comptes
À partir du plan comptable, vous pouvez ouvrir chaque compte général et ajouter ou modifier des paramètres.

**Remarque** : vous pouvez supprimer un compte général. Toutefois, avant que de le supprimer, les conditions suivantes doivent être réunies :  
- Le solde du compte doit être nul.  
- Le champ **Autoriser suppr. cpte gén. av.** doit être défini dans la fenêtre **Paramètres comptabilité**, et le compte ne doit pas comporter d'écritures comptables à cette date ou après celle-ci.  
- Si le champ **Vérifier activité cpte général** de la fenêtre **Paramètres comptabilité** est sélectionné, le compte ne doit pas être utilisé dans les groupes comptabilisation ni dans une configuration de la validation.  

Dynamics NAV vous empêchera de supprimer un compte général qui stocke les données nécessaires au plan comptable.  

##<a name="see-also"></a>Voir aussi  
[Les écritures comptables et le plan comptable](finance-setup-general-ledger.md)  
[Gérer les comptes bancaires](bank-manage-bank-accounts.md)  
[Axes analytiques](finance-setup-dimensions.md)  
[Procédure : utilisation des codes IGRF au Canada](ca-finance-setup-work-GiFI-codes.md)

