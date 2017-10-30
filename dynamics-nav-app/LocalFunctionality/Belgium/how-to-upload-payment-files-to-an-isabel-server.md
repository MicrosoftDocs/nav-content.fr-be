---
title: Comment charger les fichiers paiement sur un serveur Isabel
description: "Les fichiers paiement peuvent être chargés à l'aide de la fenêtre **Journaux IBS**. Les champs **Mode d'intégration du téléchargement (amont)** et **Mode d'intégration du téléchargement (aval)** dans la fenêtre **Configuration de la banque électronique** doivent être définis sur **Interactif** pour charger des fichiers paiement."
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
ms.openlocfilehash: d9d62008d1e3c2923d9640e3997b31ab95e76dc4
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-upload-payment-files-to-an-isabel-server"></a>Comment charger les fichiers paiement sur un serveur Isabel
Les fichiers paiement peuvent être chargés à l'aide de la fenêtre **Journaux IBS**. Les champs **Mode d'intégration du téléchargement (amont)** et **Mode d'intégration du téléchargement (aval)** dans la fenêtre **Configuration de la banque électronique** doivent être définis sur **Interactif** pour charger des fichiers paiement.  
  
> [!NOTE]  
>  Avant de pouvoir charger des fichiers paiement, vous devez vous connecter au serveur Isabel.  
  
### <a name="to-upload-payment-files-in-attended-mode"></a>Pour charger des fichiers paiement en mode interactif  
  
1.  Sélectionnez l'icône ![Rechercher une page ou un état](media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Journaux IBS**, puis sélectionnez le lien correspondant.  
  
2.  Dans l'onglet **Accueil**, dans le groupe **Processus**, sélectionnez **Extraire le contrat et l'utilisateur**.  
  
3.  Une fois les fichiers paiement vérifiés, un code utilisateur et un ID contrat s'afficheront dans les champs **Code utilisateur IBS** et **ID contrat IBS**.  
  
     Le champ **Statut du téléchargement** sera défini sur **Prêt pour téléchargement**. S'il existe plus d'un contrat sur le serveur Isabel pour le compte bancaire, le champ **Statut du téléchargement** sera défini sur **Existence d'un conflit**. Sélectionnez le contrat adéquat.  
  
4.  Dans l'onglet **Accueil**, dans le groupe **Traiter**, sélectionnez **Procéder au téléchargement**. Les fichiers paiement seront téléchargés sur le serveur Isabel et le champ **Statut du téléchargement** sera défini sur **Traité**.  
  
5.  Continuez à traiter les fichiers paiement en signant et en envoyant les fichiers sur le serveur Isabel.  
  
## <a name="see-also"></a>Voir aussi  
 Configuration de la banque électronique   
 Journaux IBS   
 [Comment archiver les écritures journal IBS](how-to-archive-ibs-log-entries.md)
