---
title: Configurer des virements SEPA
description: "Découvrez comment configurer des virements SEPA dans Dynamics NAV."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sepa, credit, transfer, payment,
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5dd85579a39fc9bfb3bb362e9573facc0c0a3977
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-sepa-credit-transfer"></a>Procédure : configurer des virements SEPA
Dans la fenêtre **Feuille paiement**, vous pouvez exporter des paiements vers un fichier pour le charger sur votre banque électronique afin de traiter les transferts d'argent liés. [!INCLUDE[d365fin](includes/d365fin_md.md)] prend en charge le format de virement SEPA, mais dans votre pays/région, d'autres formats de paiements électroniques peuvent être disponibles.  

Pour activer l'exportation de formats de fichiers bancaires qui ne sont pas pris en charge en natif dans [!INCLUDE[d365fin](includes/d365fin_md.md)], vous pouvez configurer une définition d'échange de données à l'aide de l'infrastructure d'échange de données. Pour plus d'informations, reportez vous à [Procédure : configurer les définitions d'échange de données](across-how-to-set-up-data-exchange-definitions.md).  

Avant de pouvoir traiter le paiement par voie électronique lorsque vous exportez des fichiers paiement au format de virement SEPA, vous devez exécuter les étapes de configuration suivantes :  

* Paramétrer le compte bancaire concerné pour traiter le format de virement SEPA  
* Configurer des fiches fournisseur pour traiter les paiements en exportant les fichiers au format de virement SEPA  
* Configurer la feuille comptabilité associée pour activer l'export de paiement à partir de la fenêtre **Feuille paiement**  
* Lier la définition d'échange de données pour un ou plusieurs types de règlement au(x) mode(s) de règlement approprié(s)  

### <a name="to-set-up-a-bank-account-for-sepa-credit-transfer"></a>Pour configurer un compte bancaire pour SEPA Credit Transfer  
1. Dans la zone **Rechercher**, saisissez **Comptes bancaires**, puis sélectionnez le lien associé.  
2. Ouvrez la fiche du compte bancaire à partir duquel vous exporterez des fichiers paiement au format de virement SEPA.  
3. Sur le raccourci **Transfert**, dans le champ **Format exportation paiement**, choisissez **SEPADD**.  
4. Dans le champ **Souches de n° ID Msg Virement SEPA**, sélectionnez une souche de numéros dont les numéros sont affectés aux écritures de virement SEPA.  
5. Assurez-vous que le champ **IBAN** est renseigné.  

    > [!NOTE]  
    >  Le champ **Code devise** doit avoir la valeur **EUR**, car les virements SEPA ne peuvent être effectués que dans la devise EURO.  

### <a name="to-set-up-a-vendor-card-for-sepa-credit-transfer"></a>Pour configurer une fiche fournisseur pour SEPA Credit Transfer  
1. Dans la zone **Rechercher**, entrez **Fournisseurs**, puis sélectionnez le lien associé.  
2. Ouvrez la fiche du fournisseur que vous allez payer par voie électronique en exportant des fichiers paiement au format de virement SEPA.  
3. Sur le raccourci **Paiement**, dans le champ **Code mode de règlement**, sélectionnez **BANQUE**.  
4. Dans le champ **Compte bancaire préféré**, cliquez sur la banque sur laquelle l'argent est transféré lorsqu'il est traité par votre banque électronique.  

     La valeur du champ **Compte bancaire préféré** est copiée dans le champ **Cpte bancaire destinataire** de la fenêtre **Feuille paiement**.  

### <a name="to-set-the-payment-journal-up-to-export-payment-files"></a>Pour définir la feuille de paiement jusqu'aux fichiers de paiement d'exportation  
1. Dans la zone **Rechercher**, entrez **Feuilles paiement**, puis choisissez le lien associé.  
2. Ouvrez la feuille paiement que vous utilisez pour traiter les paiements en exportant les fichiers au format de virement SEPA.  
3. Dans le champ **Nom de la feuille**, choisissez le bouton déroulant.  
4. Dans la fenêtre **Noms feuilles comptabilité**, sous l'onglet **Accueil**, dans le groupe **Gestion**, choisissez **Modifier la liste**.  
5. Sur la ligne de la feuille paiement que vous allez utiliser pour exporter des paiements, activez la case à cocher **Autoriser exportation paiement**.  

### <a name="to-connect-the-data-exchange-definition-for-one-or-more-payment-types-with-the-relevant-payment-method-or-methods"></a>Pour lier la définition d'échange de données pour un ou plusieurs types de règlement au(x) mode(s) de règlement approprié(s)  
1. Dans la zone **Rechercher**, entrez **Modes de règlement**, puis choisissez le lien associé.  
2. Dans la fenêtre **Modes de règlement**, sélectionnez le mode de paiement qui est utilisé pour exporter des paiements, puis cliquez sur le champ **Définition ligne exportation paiem.**  
3. Dans la fenêtre **Définitions ligne exportation paiem.**, sélectionnez le code spécifié dans le champ **Code** du raccourci **Définitions ligne** à l'étape 4 de la section « Pour décrire le formatage des lignes et des colonnes dans le fichier » dans la [Procédure : configurer les définitions d'échange de données](across-how-to-set-up-data-exchange-definitions.md).  

    Le mandat de prélèvement est automatiquement inséré dans le champ **ID mandat de prélèvement** lorsque vous créez une facture vente pour le client que vous avez sélectionné à l'étape 2. Pour plus d'informations, voir [Procédure : Créer des lignes vente et achat récurrentes](sales-how-work-standard-lines.md).  

## <a name="see-also"></a>Voir aussi  
[Recouvrement de paiements par prélèvement automatique SEPA](finance-collect-payments-with-sepa-direct-debit.md)  
[Procédure : configurer les définitions d'échange de données](across-how-to-set-up-data-exchange-definitions.md)  
[Procédure : Créer des lignes ventes et achat récurrentes](sales-how-work-standard-lines.md)  
[Échanger des données par voir électronique](across-data-exchange.md)  

