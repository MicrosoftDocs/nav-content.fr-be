---
title: "Procédure : activer les paiements client via Paypal"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a2268d8454af761c40b11d89b01778a3f92090fb
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a>Procédure : activer les paiements client via PayPal#
Au lieu de collecter des paiements par l'intermédiaire de transferts bancaires ou de cartes de crédit, vous pouvez proposer à vos clients de vous payer via leur compte Paypal.

Lorsqu'un client clique sur le lien Paypal sur une facture vente ou un document commande vente, la page de service de leur compte Paypal s'ouvre et affiche les détails de paiement pour la vente. Le client peut ensuite payer la facture comme tout autre paiement Paypal.

Pour activer les paiements client via Paypal, vous devez effectuer les opérations suivantes :

1. Configurer PayPal Payments Standard comme service de paiement dans la fenêtre **Services de paiement**.
2. Sélectionnez PayPal Payments Standard dans le champ **Service de paiement** du document vente en question.

Le service PayPal Payments Standard est installé comme extension de Dynamics NAV et prêt à être activé. Pour en savoir plus, voir [Personnalisation de Dynamics NAV à l'aide des extensions ](ui-extensions.md).

## <a name="to-enable-the-paypal-payments-standard-service"></a>Pour activer le service PayPal Payments Standard
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Services de paiement**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Services de paiement**, sélectionnez l'action **Nouveau**.
3. Sélectionnez **PayPal Standard**, puis fermez la fenêtre.
4. Dans la fenêtre **Services de paiement**, sélectionnez l'action **Configuration**.
5. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

    **Remarque** : cochez la case **Toujours inclure dans les documents** si vous souhaitez que le lien hypertexte pour le service de paiement Paypal soit toujours visible sur les documents vente pour lesquels le paiement par Paypal est activé.

6. Fermez la fenêtre.

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a>Pour sélectionner PayPal Payments Standard sur une facture vente
1. Sur la page d'accueil, sélectionnez **Factures vente**.
2. Ouvrez la facture vente pour laquelle vous souhaitez activer les paiements via Paypal.
3. Dans le champ **Service de paiement**, sélectionnez PayPal Payments Standard.

**Remarque** : le champ **Service de paiement** est uniquement visible si le service PayPal Payments Standard est activé.   

## <a name="see-also"></a>Voir aussi  
[Configuration des ventes](sales-setup-sales.md)  
[Gestion des ventes](sales-manage-sales.md)  
[Personnalisation de Dynamics NAV à l'aide des extensions](ui-extensions.md)

