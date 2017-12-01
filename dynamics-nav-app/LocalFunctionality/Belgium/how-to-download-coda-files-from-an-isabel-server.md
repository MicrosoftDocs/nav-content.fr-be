---
title: "Comment télécharger des fichiers CODA à partir d'un serveur Isabel"
description: "Les fichiers CODA peuvent être téléchargés manuellement ou en mode interactif."
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
ms.openlocfilehash: 28d427fbeb308ba57ee96272cf98ab9d75c06b46
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-download-coda-files-from-an-isabel-server"></a>Comment télécharger des fichiers CODA à partir d'un serveur Isabel
Les fichiers CODA peuvent être téléchargés manuellement ou en mode interactif.  

Pour télécharger manuellement des fichiers CODA, connectez-vous au serveur Isabel et sélectionnez les fichiers que vous souhaitez télécharger. Les fichiers téléchargés peuvent ensuite être importés à partir de la table **Compte bancaire**. Pour plus d'informations, voir [Comment importer des relevés CODA](how-to-import-coda-statements.md).  

## <a name="to-download-coda-files-in-attended-mode"></a>Pour télécharger des fichiers CODA en mode interactif  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Journaux IBS**, puis sélectionnez le lien correspondant.  
2.  Choisissez l'action **Télécharger**.  
3.  Dans la fenêtre **Options de demande de téléchargement IBS**, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Date début**|Spécifiez la date de début du téléchargement.|  
    |**Historique cumulé**|Spécifiez la date de fin du téléchargement.|  
    |**Format de fichier**|Sélectionnez **Coda** comme format de fichier.|  
    |**Statut du fichier**|Sélectionnez le statut du fichier du téléchargement. Les statuts du fichier incluent **Non téléchargé**, **Téléchargé** et **Tout**. Généralement, vous devez sélectionner **Non téléchargé**, car vous téléchargez les fichiers CODA qui n'ont pas été téléchargés dans votre système.|  

4.  Cliquez sur le bouton **OK**.  

    > [!NOTE]  
    >  Vous ne pouvez supprimer aucune fichier du serveur Isabel via la fenêtre **Options de demande de téléchargement IBS**. Vous devez supprimer manuellement les fichiers en vous connectant au serveur Isabel.  

     Après le téléchargement des fichiers CODA, le champ **Statut processus** sera défini sur **Créé** dans la fenêtre **Journaux IBS**. Vous pouvez vous connecter au serveur Isabel pour récupérer les fichiers manuellement. Pour plus d'informations, voir [Comment importer des relevés CODA](how-to-import-coda-statements.md).  

## <a name="see-also"></a>Voir aussi  
[Fonctionnalité locale pour la Belgique](belgium-local-functionality.md)

