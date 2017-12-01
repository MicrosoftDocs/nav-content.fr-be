---
title: Comment charger les fichiers paiement sur un serveur Isabel
description: "Les fichiers paiement peuvent être chargés à l'aide de la fenêtre **Journaux IBS**. Les champs **Mode d'intégration du téléchargement (amont)** et **Mode d'intégration du téléchargement (aval)** dans la fenêtre **Configuration de la banque électronique** doivent être définis sur **Interactif** pour charger des fichiers paiement."
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
ms.openlocfilehash: fa15bbba7beb1a90df5a6051ab763a802268da79
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-upload-payment-files-to-an-isabel-server"></a>Comment charger les fichiers paiement sur un serveur Isabel
Les fichiers paiement peuvent être chargés à l'aide de la fenêtre **Journaux IBS**. Les champs **Mode d'intégration du téléchargement (amont)** et **Mode d'intégration du téléchargement (aval)** dans la fenêtre **Configuration de la banque électronique** doivent être définis sur **Interactif** pour charger des fichiers paiement.  

> [!NOTE]  
>  Avant de pouvoir charger des fichiers paiement, vous devez vous connecter au serveur Isabel.  

## <a name="to-upload-payment-files-in-attended-mode"></a>Pour charger des fichiers paiement en mode interactif  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Journaux IBS**, puis sélectionnez le lien correspondant.  
2.  Choisissez l'action **Extraire le contrat et l'utilisateur**.  
3.  Une fois les fichiers paiement vérifiés, un code utilisateur et un ID contrat s'afficheront dans les champs **Code utilisateur IBS** et **ID contrat IBS**.  

    Le champ **Statut du téléchargement** sera défini sur **Prêt pour téléchargement**. S'il existe plus d'un contrat sur le serveur Isabel pour le compte bancaire, le champ **Statut du téléchargement** sera défini sur **Existence d'un conflit**. Sélectionnez le contrat adéquat.  

4.  Choisissez l'action **Procéder au téléchargement**. Les fichiers paiement seront téléchargés sur le serveur Isabel et le champ **Statut du téléchargement** sera défini sur **Traité**.  
5.  Continuez à traiter les fichiers paiement en signant et en envoyant les fichiers sur le serveur Isabel.  

## <a name="see-also"></a>Voir aussi  
 [Comment archiver les écritures journal IBS](how-to-archive-ibs-log-entries.md)

