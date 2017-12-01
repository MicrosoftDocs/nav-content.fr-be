---
title: "Comment classer les paiements SEPA non libellés en Euro"
description: "Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez classer les paiements SEPA non libellés en Euro avec la banque. Cette fonction est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas le format SEPA et pour des devises autres que l'euro."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 6fc38866ebc02ef0873e94fc00c2e54c268e840c
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-file-non-euro-sepa-payments"></a>Comment classer les paiements SEPA non libellés en Euro
Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez classer les paiements SEPA non libellés en Euro avec la banque. Cette fonction est utile lorsque vous effectuez des paiements vers d'autres pays qui n'utilisent pas le format SEPA et pour des devises autres que l'euro.  

Avant de classer un paiement non libellé en Euro, vous devez remplir les tâches administratives suivantes :  

- Configurer un nouveau protocole d'exportation pour un paiement SEPA non libellé en Euro. Pour plus d'informations, voir Protocole d'exportation.  
- Dans la table **Pays/Région**, effacez le champ **SEPA autorisé** pour chaque pays appartenant à la zone EEA.  
- Vérifiez que le champ **Devise Euro** de la table **Paramètres comptabilité** n'est pas en Euro.  
- Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient les codes IBAN et SWIFT.  

## <a name="to-file-a-non-euro-sepa-payment"></a>Pour classer un paiement SEPA non libellé en Euro  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Classer les paiements SEPA non libellés en Euro**, puis sélectionnez le lien correspondant.  
2.  Remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA non libellé en Euro.|  
    |**Feuille**|Spécifiez le nom feuille comptabilité pour l'état de paiement SEPA non libellé en Euro.|  
    |**Valider lignes FS**|Spécifiez si vous souhaitez transférer les lignes de paiement dans la comptabilité.|  
    |**Inclure axes**|Entrez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA non libellé en Euro. Cette option est uniquement disponible si le champ **Résumer lignes FS** de la fenêtre **Configuration de la banque électronique** est sélectionné.|  
    |**Date d'exécution**|Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date de validation sur les lignes paiement.|  
    |**Nom du fichier**|Entrez le nom du fichier, y compris le disque et le dossier, à partir duquel vous souhaitez imprimer l'état.|  

3.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Comment classer les paiements SEPA](how-to-file-sepa-payments.md)   
 [Comment activer les paiements SEPA](how-to-activate-sepa-payments.md)   
 [Paiements SEPA](sepa-payments.md)

