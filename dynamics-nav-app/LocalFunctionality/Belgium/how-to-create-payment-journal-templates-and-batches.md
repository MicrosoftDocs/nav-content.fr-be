---
title: "Comment créer des modèles et lots feuille paiement"
description: "Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], des propositions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est semblable à celle des autres types de feuilles."
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
ms.openlocfilehash: 2134226936e733f0756249436c5cb77f56a125d4
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-payment-journal-templates-and-batches"></a>Comment créer des modèles et lots feuille paiement
Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], des propositions de paiement sont générées et validées dans les feuilles paiement. La structure de la feuille paiement est semblable à celle des autres types de feuilles. Toutefois, la feuille paiement contient des champs spécifiques au traitement des paiements. Avant de pouvoir commencer à générer des propositions de paiement, vous devez configurer un modèle feuille paiement et un nom feuille paiement.  

Si vous attribuez un compte bancaire au modèle feuille paiement, le compte bancaire sera inséré dans tous les noms feuille paiement et toutes les lignes feuille paiement créés à l'aide de ce modèle. En indiquant un compte bancaire pour le modèle feuille, vous pouvez réduire le délai de vérification des propositions de paiement.  

## <a name="to-create-a-payment-journal-template"></a>Pour créer un modèle feuille paiement  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Modèles FS paiements**, puis sélectionnez le lien correspondant.  
2.  Choisissez l'action **Nouveau**.  
3.  Dans la fenêtre **Modèles FS paiements EB**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom**|Entrez le nom unique du modèle feuille paiement que vous créez.|  
    |**Description**|Entrez une description du modèle feuille paiement.|  
    |**Compte bancaire**|Sélectionnez le compte bancaire qui sera utilisé lorsque vous créerez une proposition de paiement.|  
    |**Code motif**|Sélectionnez le code motif qui sera utilisé sur tous les noms et lignes feuille créés à l'aide du modèle feuille. Si vous souhaitez utiliser un autre code motif sur une ligne feuille, vous pouvez le modifier manuellement.|  
    |**Code journal**|Sélectionnez le code source qui sera utilisé sur tous les noms et lignes feuille créés à l'aide du modèle feuille.|  

4.  Cliquez sur le bouton **OK**.  

## <a name="to-add-payment-journal-batches-to-the-journal-template"></a>Pour ajouter des noms feuille paiement au modèle feuille  

1.  Dans la fenêtre **Modèles FS paiements**, choisissez l'action **Noms feuilles**.  
2.  Dans la fenêtre **Nom FS paiements**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Spécifiez un nom de modèle feuille pour le nom feuille paiement.|  
    |**Nom**|Entrez un nom unique pour le nom feuille.<br /><br /> **NOTE :** pour que le nom feuille se mette à jour de façon numérique, ajoutez un numéro dans le nom feuille. Par exemple, à chaque validation, le nom KBC1 sera mis à jour en KBC2, KBC3, etc.|  
    |**Description**|Entrez une description pour le nom feuille.|  
    |**Code motif**|Spécifie le code motif lié à ce nom feuille.|  
    |**Statut**|Indique le statut du lot.|  

3.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Comment configurer la banque électronique](how-to-set-up-electronic-banking.md)   
 [Comment configurer les codes transaction IBLC/BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)

