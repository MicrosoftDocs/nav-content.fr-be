---
title: "Comment générer des propositions de paiement"
description: "Après avoir configuré la banque électronique, vous pouvez commencer à générer des propositions de paiement. Vous pouvez le faire dans la feuille paiement."
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
ms.openlocfilehash: 4b677e113d98477d9a2a34af57cb06c285e8eb6c
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-generate-payment-suggestions"></a>Comment générer des propositions de paiement
Après avoir configuré la banque électronique, vous pouvez commencer à générer des propositions de paiement. Vous pouvez le faire dans la feuille paiement.  
  
### <a name="to-generate-payment-suggestions"></a>Pour générer des propositions de paiement  
  
1.  Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Feuilles paiement**, puis sélectionnez le lien correspondant.  
  
2.  Sélectionnez la feuille adéquate, puis, dans l'onglet **Accueil**, dans le groupe **Progression**, sélectionnez **Proposer paiements fournisseur**.  
  
3.  Dans la fenêtre **Proposer paiements fournisseur**, dans le raccourci **Options**, remplissez les champs comme indiqué dans le tableau suivant.  
  
    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Dern. date d'échéance**|Entrez la dernière date d'échéance qui peut apparaître sur les écritures comptables fournisseur à inclure dans le traitement par lots.|  
    |**Tenir compte des avoirs**|Sélectionnez pour inclure les avoirs restants pour les fournisseurs. Les avoirs seront soustraits du montant dû. Lorsque vous sélectionnez des avoirs, la date d'échéance n'est pas utilisée.|  
    |**Obtenir escomptes**|Sélectionnez pour inclure les écritures comptables fournisseur pour lesquelles vous pouvez obtenir un escompte.|  
    |**Date d'escompte**|Entrez la date qui sera utilisée pour calculer un escompte.|  
    |**Montant disponible**|S'il y a un montant maximal disponible pour les paiements, vous pouvez l'entrer ici. Le traitement par lots créera alors une proposition de paiement basée sur ce montant et la priorité des fournisseurs.|  
    |**Date comptabilisation**|Entrez la date qui apparaîtra comme date de validation sur les lignes que le traitement par lots insère dans la feuille paiement.|  
  
4.  Dans le raccourci **Fournisseur**, entrez les critères de filtre.  
  
5.  Cliquez sur le bouton **OK** pour démarrer le traitement par lots.  
  
     Lorsque le traitement par lots est terminé, la feuille paiement contient toutes les écritures comptables fournisseur qui correspondent aux filtres.  
  
## <a name="see-also"></a>Voir aussi  
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Comment configurer les fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Comment créer des modèles et lots feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Comment tester les paiements électroniques](how-to-test-electronic-payments.md)   
 [Comment gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md)   
 [Comment imprimer les fichiers paiement](how-to-print-payment-files.md)
