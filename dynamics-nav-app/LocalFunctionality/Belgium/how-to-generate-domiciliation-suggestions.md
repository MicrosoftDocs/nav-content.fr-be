---
title: "Comment générer des propositions de domiciliation"
description: "Après avoir configuré des domiciliations, vous pouvez commencer à générer des propositions de domiciliation. Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez uniquement créer des propositions de domiciliation pour des clients nationaux."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 20006ba794abeffeaecc7d36d1113469a464c3ab
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-generate-domiciliation-suggestions"></a>Comment générer des propositions de domiciliation
Après avoir configuré des domiciliations, vous pouvez commencer à générer des propositions de domiciliation. Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez uniquement créer des propositions de domiciliation pour des clients nationaux.  

## <a name="to-generate-domiciliation-suggestions"></a>Pour générer des propositions de domiciliation  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuille saisie domiciliation**, puis sélectionnez le lien correspondant.  
2.  Dans le champ **Nom feuille**, sélectionnez la feuille concernée, puis choisissez l'action **Proposer domiciliations**.  
3.  Dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Date besoin**|Entrez la date d'échéance à inclure dans le traitement par lots. Seules les écritures ayant une date d'échéance antérieure ou identique à cette date seront incluses.|  
    |**Obtenir escomptes**|Sélectionnez si vous souhaitez que le traitement par lots comprenne les écritures comptables client pour lesquelles vous pouvez obtenir un escompte.|  
    |**Date d'escompte**|Entrez la date qui sera utilisée pour calculer l'escompte.|  
    |**Inclure remboursements poss.**|Sélectionnez si vous souhaitez que le traitement par lots inclue les remboursements.|  
    |**Date comptabilisation**|Entrez la date qui apparaîtra comme date de validation sur les lignes que le traitement par lots insère dans la feuille domiciliation.|  

4.  Dans le raccourci **Client**, entrez les éventuels critères de filtre supplémentaires.  
5.  Cliquez sur le bouton **OK**.  

Lorsque le traitement par lots est terminé, la feuille domiciliation contient toutes les écritures comptables client ouvertes qui correspondent aux filtres.  

> [!NOTE]  
>  Les propositions de domiciliation incluront uniquement les clients qui ont un numéro de domiciliation configuré. Pour plus d'informations, voir [Comment configurer des domiciliations](how-to-set-up-domiciliations.md).  

## <a name="see-also"></a>Voir aussi  
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Domiciliation européenne](direct-debit-using-domiciliation.md)   
 [Comment configurer des domiciliations](how-to-set-up-domiciliations.md)   
 [Comment tester les domiciliations](how-to-test-domiciliations.md)   
 [Comment modifier et supprimer des lignes domiciliation](how-to-edit-and-delete-domiciliation-lines.md)   
 [Comment exporter et valider des domiciliations](how-to-export-and-post-domiciliations.md)

