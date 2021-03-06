---
title: "Procédure : configurer des clients effectuant un achat au comptoir"
description: "Cette rubrique décrit les étapes pour configurer un client qui paie en espèces."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/11/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: dca1e2b58d22a9d27766a731a085278f1200b570
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-cash-customers"></a>Procédure : configurer des clients effectuant un achat au comptoir
Vous ne pouvez pas créer une facture sans numéro de client. Ceci est valable même si vous effectuez une vente au comptoir et que vous n'avez rien à enregistrer dans un compte client.  

## <a name="to-set-up-a-cash-customer"></a>Pour configurer des clients effectuant un achat en espèces  
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Client**, puis sélectionnez le lien connexe.  
2.  Créez une fiche **Client**. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux clients](sales-how-register-new-customers.md).
3.  Dans le champ **N°**, , saisissez par exemple **Espèces**.  
4.  Dans le champ **Nom**, saisissez par exemple **Vente au comptoir**.  
5.  Sur le raccourcie **Facturation**, renseignez les champs **Groupe compta. client** et **Groupe compta. marché**.  

 Vous avez alors configuré un client contenant suffisamment d'informations de facturation.  

> [!NOTE]  
>  Vous avez peut-être choisi un groupe comptabilisation également utilisé pour les ventes à crédit nationales. Si vous souhaitez mettre à jour des données séparées sur les ventes au comptoir, par exemple avec un compte client ou fournisseur spécial, vous pouvez configurer un groupe comptabilisation supplémentaire à cet effet.  
>   
>  Vous devez saisir le numéro d'un compte client pour le groupe comptabilisation, même si le solde de ce compte est toujours de 0 après la validation d'une facture.  

## <a name="see-also"></a>Voir aussi
[Gestion des comptes client](receivables-manage-receivables.md)  
[Procédure : enregistrer de nouveaux clients](sales-how-register-new-customers.md)    
[Finances](finance.md)  


