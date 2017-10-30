---
title: Comment classer les paiements SEPA
description: Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez utiliser les virements de type SEPA (Single Euro Payments Area) pour classer les paiements SEPA avec la banque.
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 27bdc9a6616fc89a8e8d755a57439855b97701bf
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-file-sepa-payments"></a>Comment classer les paiements SEPA
Dans [!INCLUDE[navnow](../../includes/navnow_md.md)], vous pouvez utiliser les virements de type SEPA (Single Euro Payments Area) pour classer les paiements SEPA avec la banque.  
  
 Le format SEPA unifie les modes de paiement des pays/régions européens participants, ce qui rend les paiements internationaux aussi faciles à traiter que les paiements nationaux. Les citoyens et les sociétés européens peuvent effectuer et recevoir des paiements en euros, dans ou au-delà des frontières nationales, avec les mêmes conditions, droits et obligations de base, quel que soit l'emplacement.  
  
 Avant de classer un paiement, vous devez remplir les tâches administratives suivantes :  
  
-   Configurer un nouveau protocole d'exportation. Pour plus d'informations, voir Protocole d'exportation.  
  
-   Dans la table **Pays/Région**, sélectionnez le champ **SEPA autorisé** pour chaque pays appartenant à la zone EEA.  
  
-   Vérifiez que le champ **Devise Euro** de la table **Paramètres comptabilité** correspond à la devise sur les lignes paiement.  
  
-   Vérifiez que le champ **Compte bancaire préféré** du fournisseur dans la table **Fournisseur** contient les codes IBAN et SWIFT.  
  
### <a name="to-file-a-sepa-payment"></a>Pour classer un paiement SEPA  
  
1.  Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Classer les paiements SEPA**, puis sélectionnez le lien correspondant.  
  
2.  Remplissez les champs comme indiqué dans le tableau suivant.  
  
    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom modèle feuille**|Spécifiez le modèle feuille comptabilité pour l'état de paiement SEPA.|  
    |**Feuille**|Spécifiez le nom feuille comptabilité pour l'état de paiement SEPA.|  
    |**Valider lignes FS**|Spécifiez si vous souhaitez transférer les lignes de paiement dans la comptabilité.|  
    |**Inclure axes**|Entrez les axes analytiques que vous souhaitez inclure dans l'état de paiement SEPA. Cette option est uniquement disponible si le champ **Résumer lignes FS** de la fenêtre **Configuration de la banque électronique** est sélectionné.|  
    |**Date d'exécution**|Entrez une date d'exécution si vous souhaitez que la date d'exécution soit différente de la date de validation sur les lignes paiement.|  
    |**Nom du fichier**|Entrez le nom du fichier, y compris le disque et le dossier, à partir duquel vous souhaitez imprimer l'état.|  
  
3.  Cliquez sur le bouton **OK**.  
  
## <a name="see-also"></a>Voir aussi  
 Classer les paiements SEPA   
 [Comment configurer des protocoles d'exportation](how-to-set-up-export-protocols.md)   
 Protocole d'exportation   
 [Comment classer les paiements SEPA non libellés en Euro](how-to-file-non-euro-sepa-payments.md)   
 [Comment activer les paiements SEPA](how-to-activate-sepa-payments.md)
