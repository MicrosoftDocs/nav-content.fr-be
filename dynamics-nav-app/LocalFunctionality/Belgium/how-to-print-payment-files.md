---
title: Comment imprimer les fichiers paiement
description: "Après avoir imprimé un test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier paiement."
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
ms.openlocfilehash: 49936b0396a4c52ca78d150feeeeaff96c149ae9
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-print-payment-files"></a>Comment imprimer les fichiers paiement
Après avoir imprimé un test et corrigé toutes les erreurs, vous pouvez imprimer les lignes feuille paiement dans un fichier paiement.  

Un fichier paiement contient des paiements nationaux, internationaux, SEPA ou SEPA non libellés en Euro. Le fichier peut être envoyé à une banque sur disquette, par un modem ou via Isabel (Interbanks Standards Association Belgium). Vous ne pouvez créer qu'un fichier par date de validation et par code devise. Lorsque vous exportez les paiements dans un fichier, une note d'accompagnement est imprimée et peut aussi être envoyée à la banque.  

Dans la feuille paiement, le champ **Statut** des lignes exportées sera défini sur **Validé**.  

## <a name="to-print-a-payment-file"></a>Pour imprimer un fichier paiement  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuille paiement**, puis sélectionnez le lien correspondant.  
2.  Dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom de la feuille**|Spécifiez le nom de la feuille paiement.|  
    |**Compte bancaire**|Spécifiez le compte bancaire de la feuille paiement.|  
    |**Protocole d'exportation**|Spécifiez le code du protocole d'exportation de la ligne feuille paiement. Exportez des protocoles qui contrôlent le fichier de paiement qui sera généré dans la feuille paiement.<br /><br /> Vous pouvez avoir plusieurs formats d'exportation différents dans un seul lot, comme les formats national, international, SEPA, ou un ensemble des trois. Toutefois, lorsque vous exportez les lignes paiement dans un fichier, vous ne pouvez utiliser qu'un format ou protocole d'exportation. **Note :**  En définissant le protocole d'exportation, vous définissez également le type de validation qui sera effectuée dans la feuille paiement.|  

3.  Choisissez l'action **Vérifier les lignes de paiement**.

    La fenêtre **Exporter les journaux d'erreur de chèque** affiche les erreurs éventuelles qui pourraient exister. S'il y a des erreurs, vous devez les corriger avant de continuer.

4. S'il n'y a pas d'erreur, choisissez l'action **Exporter les lignes de paiement**.  

    L'état que vous avez spécifié dans le champ **ID impression test** des **Modèles FS paiements EB** s'ouvre.  

5.  Cliquez sur le bouton **Imprimer**.  

## <a name="see-also"></a>Voir aussi  
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Comment configurer la banque électronique](how-to-set-up-electronic-banking.md)   
 [Comment configurer les codes transaction IBLC/BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Comment configurer les fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Comment générer des propositions de paiement](how-to-generate-payment-suggestions.md)   
 [Comment créer des modèles et lots feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Comment tester les paiements électroniques](how-to-test-electronic-payments.md)   
 [Comment gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md)

