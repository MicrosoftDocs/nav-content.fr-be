---
title: Comment activer les paiements SEPA
description: "Pour soumettre les paiements fournisseur par voie électronique au format de paiement Single Euro Payments Area (SEPA) ISO 20022, vous devez configurer des conditions préalables pour l'activation des paiements SEPA."
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
ms.openlocfilehash: 821039217519d2f066c842aca76687a98ae5d48d
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-activate-sepa-payments"></a>Comment activer les paiements SEPA
Pour soumettre les paiements fournisseur par voie électronique au format de paiement Single Euro Payments Area (SEPA) ISO 20022, vous devez configurer des conditions préalables pour l'activation des paiements SEPA.  
  
 Les procédures suivantes sont consacrées à l'activation d'un paiement SEPA et à la configuration de comptes bancaires fournisseur.  
  
### <a name="to-enable-countriesregions-for-sepa"></a>Pour activer des pays/régions pour SEPA  
  
1.  Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Pays/Régions**, puis sélectionnez le lien correspondant.  
  
2.  Sous l'onglet **Accueil**, dans le groupe **Gérer**, sélectionnez **Modifier la liste**.  
  
3.  Activez la case à cocher **SEPA autorisé** pour chaque pays ou région que vous souhaitez activer pour SEPA.  
  
4.  Cliquez sur le bouton **OK**.  
  
### <a name="to-enable-bank-accounts-for-sepa"></a>Pour activer des comptes bancaires pour SEPA  
  
1.  Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.  
  
2.  Sélectionnez le compte bancaire que vous souhaitez activer pour SEPA, puis, dans l'onglet **Accueil**, dans le groupe **Gérer**, sélectionnez **Modifier**.  
  
3.  Dans le raccourci **Général**, dans le champ **Pays/Région**, sélectionnez le code adéquat.  
  
    > [!NOTE]  
    >  Le code pays/région spécifié doit être activé pour SEPA, comme décrit dans la procédure précédente.  
  
4.  Entrez une valeur dans le champ **Solde minimum**.  
  
5.  Dans le raccourci **Transfert**, dans le champs **Code SWIFT**, entrez un code.  
  
6.  Cliquez sur le bouton **OK**.  
  
### <a name="to-set-up-vendor-bank-accounts-for-sepa"></a>Pour configurer des comptes bancaires fournisseur pour SEPA  
  
1.  Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Fournisseurs**, puis sélectionnez le lien correspondant.  
  
2.  Sélectionnez le fournisseur concerné, puis, dans l'onglet **Naviguer**, dans le groupe **Fournisseur**, sélectionnez **Comptes bancaires**.  
  
3.  Sélectionnez le compte bancaire fournisseur à configurer pour SEPA, puis, dans l'onglet **Accueil**, dans le groupe **Gérer**, sélectionnez **Modifier**.  
  
4.  Dans le raccourci **Transfert**, dans les champs **IBAN** et **Code SWIFT**, entrez le code international d'identification bancaire ou la banque auprès de laquelle le fournisseur a son compte.  
  
5.  Cliquez sur le bouton **OK**.  
  
## <a name="see-also"></a>Voir aussi  
 [Paiements SEPA](sepa-payments.md)   
 [Comment classer les paiements SEPA](how-to-file-sepa-payments.md)   
 [Comment classer les paiements SEPA non libellés en Euro](how-to-file-non-euro-sepa-payments.md)   
 [Comment configurer des protocoles d'exportation](how-to-set-up-export-protocols.md)
