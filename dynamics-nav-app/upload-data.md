---
title: "Importer des données à partir d'autres systèmes financiers"
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: b5bd6092046f9a8d75498ddcf3b1ce73f674e687
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="import-data-from-other-finance-systems"></a>Importer des données à partir d'autres systèmes financiers
Dans Dynamics NAV, vous pouvez choisir de créer une société vide afin de pouvoir télécharger les données d'autres systèmes financiers à utiliser dans votre nouvelle société Dynamics NAV. En fonction de la solution financière qu'utilise votre société aujourd'hui, vous pouvez transférer des informations sur les clients, les fournisseurs, le stock et les comptes bancaires.
Dans la pile Propriétaire d'entreprise du tableau de bord, vous pouvez lancer un guide de configuration assistée qui vous aide à transférer les données d'entreprise à partir d'un fichier Excel ou d'autres formats. Le type de fichiers que vous pouvez télécharger dépend des extensions disponibles. Par exemple, vous pouvez télécharger des données à partir de QuickBooks, car Dynamics NAV comprend une extension qui gère la conversion à partir de QuickBooks. Si vous souhaitez télécharger des données à partir d'autres solutions financières, vous devez vérifier qu'un extension est disponible pour cette solution ou effectuer l'importation à partir d'Excel.  
Dynamics NAV inclut des modèles pour les clients, les fournisseurs et les articles en stock, que vous pouvez choisir d'appliquer lorsque vous téléchargez vos données.  

## <a name="transfer-from-quickbooks"></a>Transfert à partir de QuickBooks
Si votre entreprise utilise QuickBooks aujourd'hui, vous pouvez exporter les informations appropriées vers un fichier IIF (Intuit Interchange Format). Vous pouvez ensuite ouvrir le guide de configuration assistée pour transférer les données.
Par exemple, si votre fichier IIF inclut les clients et les fournisseurs, vous pouvez choisir de transfert uniquement les données client. Vous pouvez alors transférer le reste des informations ultérieurement.  
La configuration assistée comprend une option permettant de modifier la configuration par défaut du transfert, mais nous vous recommandons de vous attaquer à cette configuration avancée si vous êtes familier des tables de base de données. Pour l'immense majorité des sociétés, le mappage par défaut de QuickBooks vers Dynamics NAV transfère les informations que vous souhaitez.

## <a name="see-also"></a>Voir aussi
[Finance](finance-setup.md)  
[Personnalisation de Dynamics NAV à l'aide des extensions](ui-extensions.md)   
[Configurer votre solution Dynamics NAV](setup.md)

