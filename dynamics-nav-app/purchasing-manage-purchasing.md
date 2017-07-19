---
title: Gestion des achats
author: SorenGP
ms.custom: na
ms.date: 11/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: df94e447d7d4542f75f3c34105099016b0abbf32
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="manage-purchasing"></a>Gestion des achats
Vous créez une facture achat ou une commande achat pour enregistrer le coût d'achats et suivre les créances. Si vous devez contrôler un stock, les factures achat sont également utilisées pour mettre à jour de manière dynamique les niveaux de stock afin que vous puissiez réduire vos coûts et fournir un meilleur service client. Le prix d'achat, notamment les frais de service, et les valeurs de stocks qui résultent de la validation des factures achat contribuent aux chiffres du profit et à d'autres KPI financiers sur votre page d'accueil.

Vous devez utiliser les commandes achat si votre processus de vente exige que vous enregistriez des réceptions partielles d'une quantité de commande, par exemple, si la quantité totale n'était pas disponible auprès du fournisseur. Si vous commercialisez des articles en les livrant directement depuis votre fournisseur auprès de votre client, vous devez également utiliser les commandes achat. Pour plus d'informations, voir [Procédure : effectuer des livraisons directes](sales-how-drop-shipment.md). Pour tous les autres aspects, les commandes achat fonctionnent de la même manière que les factures achat.

Les factures achat peuvent être créées automatiquement en utilisant le service de reconnaissance optique de caractères (OCR) pour convertir les factures PDF de vos fournisseurs en documents électroniques qui sont ensuite convertis en factures achat par un flux de travail. Pour utiliser cette fonctionnalité, vous devez d'abord vous inscrire au service OCR, puis effectuer diverses configurations. Pour plus d'informations, reportez vous à [Procédure : traiter les documents entrants](across-process-income-documents.md).      

**Remarque** : dans Dynamics NAV, un produit est désigné par le terme « article ».

Les produits peuvent être des articles en stock et des services. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md).

Pour tous les processus d'achat, vous pouvez incorporer un flux de travail d'approbation, par exemple, pour exiger que les achats en grande quantité soient approuvés par le responsable de la comptabilité. Pour plus d'informations, reportez-vous à [Procédure : utilisation des flux d'approbation](across-how-use-approval-workflows.md).

Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent. Ces tâches sont répertoriées dans l'ordre de leur exécution en règle générale.


|Pour |Voir |
|---|----|
|Créer une facture achat pour enregistrer votre accord avec un fournisseur pour acheter des biens selon certaines conditions de livraison et de paiement. |[Procédure : enregistrer des achats](purchasing-how-record-purchases.md)|
|Créer une facture achat pour toutes les lignes ou pour les lignes sélectionnées sur une facture vente.|[Procédure : acheter des produits pour une vente](purchasing-how-purchase-products-sale.md)|
|Créer un avoir achat pour rembourser une facture achat validée spécifique pour indiquer les produits que vous retournez au fournisseur et le montant règlement que vous récupérez.|[Procédure : traiter les retours ou annulations d'achats](purchasing-how-process-purchase-returns-cancellations.md)|
|Créer une fiche fournisseur pour chaque fournisseur auquel vous achetez des biens.|[Procédure : enregistrer de nouveaux fournisseurs](purchasing-how-register-new-vendors.md)|

## <a name="see-also"></a>Voir aussi
[Configuration des procédures achat](purchasing-setup-purchasing.md)  
[Gestion des comptes fournisseur](payables-manage-payables.md)    
[Utiliser Dynamics NAV](ui-work-product.md)  
[Fonctionnalités communes aux différents secteurs d'activité](ui-across-business-areas.md)

