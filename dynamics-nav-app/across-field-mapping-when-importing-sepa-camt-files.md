---
title: Mappage de champs lors de l'importation de fichiers SEPA CAMT
description: "Dans les marchés européens, vous pouvez importer des fichiers de relevé bancaire selon les normes régionales SEPA (Espace unique de paiement en euros)."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: bf5f65ae5535f765a93c32fee89b80cb9f79b09f
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="field-mapping-when-importing-sepa-camt-files"></a>Mappage de champs lors de l'importation de fichiers SEPA CAMT
[!INCLUDE[d365fin](includes/d365fin_md.md)] prend en charge les normes régionales SEPA (Espace unique de paiement en euros) pour importer les relevés bancaires SEPA (format CAMT). Pour plus d'informations, reportez-vous à [Procédure: configurer le service de conversion de données bancaires](bank-how-setup-bank-data-conversion-service.md).  

 La norme SEPA CAMT standard présente elle-même des variations locales. Par conséquent, vous pouvez être amené à modifier la définition d'échange de données générique (représentée par le code **SEPA CAMT** dans la fenêtre **Définitions échange comptabilité**) pour l'adapter à une variation locale de la norme. Les tables suivantes indiquent la correspondance entre élément et champ pour les tables 81, 273 et 274 dans l'implémentation de SEPA CAMT dans [!INCLUDE[d365fin](includes/d365fin_md.md)].  

 Pour plus d'informations sur la création ou l'ajustement de définition d'échange de données, reportez\-vous à [Procédure : configurer les définitions d'échange de données](across-how-to-set-up-data-exchange-definitions.md)  

## <a name="camt-data-mapping-to-fields-in-the-general-journal-table-81"></a>Association des données de CAMT avec les champs du tableau Feuille comptabilité (81)  

|Chemin d'accès d'articles|Élément message|Type de données|Désignation|Identifiant signe négatif|N° champ|Nom du champ|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|Stmt/Ntry/Amt|Montant|Décimale|Le montant de l'argent dans l'écriture de caisse.||13|Montant|  
|Stmt/Ntry/CdtDbtInd|CreditDebitIndicator|Texte.|Indique si l'écriture est une écriture de crédit ou débit|DBIT|13|Montant|  
|Stmt/Ntry/BookgDt/Dt|Date|Date|Date à laquelle une écriture est validée dans un compte sur les livres de compte du gestionnaire||5|Date comptabilisation|  
|Stmt/Ntry/BookgDt/DtTm|DateTime|DateTime|La date et l'heure auxquelles une écriture est validée dans un compte sur les livres de compte du gestionnaire||5|Date comptabilisation|  
|Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm|Nom|Texte.|Le nom de la partie qui doit une somme d'argent au créancier (final)||1 221|Informations payeur|  
|Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd|Non structuré|Texte.|Les informations à votre disposition pour activer la correspondance/le rapprochement d'une écriture avec les articles que le paiement doit régler, telles que les factures commerciales dans un système comptes-clients, sous forme non structurée||8|Désignation|  
|Stmt/Ntry/AddtlNtryInf|AdditionalEntryInformation|Texte.|Informations supplémentaires sur l'écriture.||1 222|Informations transaction|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-table-273"></a>Association des données de CAMT avec les champs du tableau Rapprochement bancaire (273)  

|Chemin d'accès d'articles|Élément message|Type de données|Désignation|Identifiant signe négatif|N° champ|Nom du champ|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|Stmt/CreDtTm|CreationDateTime|Date|Date et heure de création du message||3|Date relevé|  
|Stmt/Bal/Amt|Montant|Décimale|Le montant résultant des montants ajustés pour toutes les écritures débit et crédit||4|Solde final du relevé|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-line-table-274"></a>Association des données de CAMT avec les champs du tableau Ligne rapprochement bancaire (274)  

|Chemin d'accès d'articles|Élément message|Type de données|Désignation|Identifiant signe négatif|N° champ|Nom du champ|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|Stmt/Ntry/Amt|Montant|Décimale|Le montant de l'argent dans l'écriture de caisse.||7|Montant relevé|  
|Stmt/Ntry/CdtDbtInd|CreditDebitIndicator|Texte.|Indique si l'écriture est une écriture de crédit ou débit|DBIT|7|Montant relevé|  
|Stmt/Ntry/BookgDt/Dt|Date|Date|Date à laquelle une écriture est validée dans un compte sur les livres de compte du gestionnaire||5|Date transaction|  
|Stmt/Ntry/BookgDt/DtTm|DateTime|DateTime|La date et l'heure auxquelles une écriture est validée dans un compte sur les livres de compte du gestionnaire||5|Date transaction|  
|Stmt/Ntry/ValDt/Dt|Date|Date|Date à laquelle les immobilisations sont disponibles pour le propriétaire du compte en cas d'écriture créditrice, ou cessent d'être disponibles pour le propriétaire du compte en cas d'écriture débitrice||12|Date de valeur|  
|Stmt/Ntry/ValDt/DtTm|DateTime|DateTime|La date et l'heure auxquelles les immobilisations sont disponibles pour le propriétaire du compte en cas d'écriture créditrice, ou cessent d'être disponibles pour le propriétaire du compte en cas d'écriture débitrice||12|Date de valeur|  
|Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm|Nom|Texte.|Le nom de la partie qui doit une somme d'argent au créancier (final)||15|Informations payeur|  
|Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd|Non structuré|Texte.|Les informations à votre disposition pour activer la correspondance/le rapprochement d'une écriture avec les articles que le paiement doit régler, telles que les factures commerciales dans un système comptes-clients, sous forme non structurée||6|Désignation|  
|Stmt/Ntry/AddtlNtryInf|AdditionalEntryInformation|Texte.|Informations supplémentaires sur l'écriture.||16|Informations transaction|  

 Les articles dans le nœud **Ntry** qui sont importés dans [!INCLUDE[d365fin](includes/d365fin_md.md)] mais ne sont associés à aucun champ sont stockés dans la table **Définition colonne échange comptabilité**. Les utilisateurs peuvent afficher ces éléments des fenêtres **Feuille rapprochement bancaire**, **Lettrage paiement** et **Rapprochement bancaire** en choisissant l'action **Détails lignes de relevé bancaire**. Pour plus d'informations, reportez-vous à [Procédure : rapprocher les paiements à l'aide de l'application automatique](receivables-how-reconcile-payments-auto-application.md).  
## <a name="see-also"></a>Voir aussi  
[Configuration de l'échange de données](across-set-up-data-exchange.md)  
[Échanger des données par voir électronique](across-data-exchange.md)  
[Procédure : configurer le service de conversion de données bancaires](bank-how-setup-bank-data-conversion-service.md)   
[Procédure : Utiliser des schémas XML pour préparer des définitions d'échange de données](across-how-to-use-xml-schemas-to-prepare-data-exchange-definitions.md)  
[Procédure : rapprocher les paiements à l'aide du lettrage automatique](receivables-how-reconcile-payments-auto-application.md)  

