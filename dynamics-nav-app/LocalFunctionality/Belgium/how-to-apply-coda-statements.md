---
title: "Comment lettrer les relevés CODA"
description: "Après l'importation d'un relevé CODA, vous pouvez accéder aux lignes relevé à partir de la fenêtre **Fiche compte bancaire**. Le statut lettrage de chaque ligne sera vide, car les montants du relevé n'ont pas été lettrés à des écritures comptables en attente."
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
ms.openlocfilehash: 9c22f28cf9693bc0fec118d4783d496ac38f8187
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-apply-coda-statements"></a>Comment lettrer les relevés CODA
Après l'importation d'un relevé CODA, vous pouvez accéder aux lignes relevé à partir de la fenêtre **Fiche compte bancaire**. Le statut lettrage de chaque ligne sera vide, car les montants du relevé n'ont pas été lettrés à des écritures comptables en attente.  

Les montants du relevé peuvent être lettrés à des écritures comptables en attente des manières suivantes :  

-   Lettrage manuel des lignes relevé CODA.  
-   Lettrage automatique des montants du relevé CODA aux écritures comptables et comptes adéquats. Le traitement automatique des lignes relevé CODA est recommandé.  

## <a name="to-manually-apply-the-coda-statement-lines"></a>Pour lettrer manuellement les lignes relevé CODA  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.  
3.  Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.  
4.  Dans le raccourci **Lignes relevé CODA**, pour chaque ligne relevé, remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**N° compte**|Entrez le numéro du compte général, la banque, le client, le fournisseur ou l'immobilisation auquel la ligne relevé compte bancaire est liée.|  
    |**Description**|[!INCLUDE[navnow](../../includes/navnow_md.md)] récupère automatiquement la description à partir du fichier CODA importé, mais vous pouvez modifier le contenu de ce champ.|  

5.  Cliquez sur le bouton **OK**.  

## <a name="to-automatically-apply-the-coda-statement-lines"></a>Pour lettrer automatiquement les lignes relevé CODA  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Comptes bancaires**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez le compte bancaire, puis choisissez l'action **Relevés CODA**.  
3.  Sélectionnez le relevé CODA, puis choisissez l'action **Modifier**.  
4.  Choisissez l'action **Valider lignes relevé CODA**.  
5.  Remplissez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Validation par défaut**|Définissez si vous souhaitez que le traitement par lots valide les montants du relevé qui ne peuvent pas être liés à des écritures comptables existantes. Pour plus d'informations, voir Encodage CODA.|  
    |**Imprimer liste**|Sélectionnez l'option d'impression d'une liste des montants du relevé qui ne peuvent pas être liés automatiquement.|  

6.  Cliquez sur le bouton **OK**.  

    Lorsque vous commencez le traitements par lots, les montants du relevé seront lettrés à des écritures comptables existantes selon les codes transaction. Pour plus d'informations, voir [Comment configurer des comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md).  

## <a name="see-also"></a>Voir aussi  
 [Relevés bancaires CODA](coda-bank-statements.md)   
 [Comment configurer les comptes bancaires pour CODA](how-to-set-up-bank-accounts-for-coda.md)   
 [Comment configurer les codes transaction IBLC/BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Comment importer les relevés CODA](how-to-import-coda-statements.md)   
 [Comment créer des feuilles financières](how-to-create-financial-journals.md)   
 [Comment transférer et valider automatiquement les relevés CODA](how-to-automatically-transfer-and-post-coda-statements.md) .   
 [Comment transférer et valider manuellement les relevés CODA](how-to-manually-transfer-and-post-coda-statements.md).

