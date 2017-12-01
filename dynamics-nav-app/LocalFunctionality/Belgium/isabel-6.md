---
title: Isabel 6
description: "L'organisation Isabel a développé une plateforme appelée Client Isabel Synchronizer (CIS), qui permet l'intégration sécurisée de [!INCLUDE[navnow](../../includes/navnow_md.md)] avec Isabel. CIS traite les échanges de documents depuis et vers le serveur Isabel."
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
ms.openlocfilehash: 38b27c23fc7d9223e2185b087b044bb19bdbd4b4
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="isabel-6"></a>Isabel 6
L'organisation Isabel a développé une plateforme appelée Client Isabel Synchronizer (CIS), qui permet l'intégration sécurisée de [!INCLUDE[navnow](../../includes/navnow_md.md)] avec Isabel. CIS traite les échanges de documents depuis et vers le serveur Isabel.  

Pour télécharger les fichiers bancaires depuis ou vers le serveur, vous devez configurer votre environnement pour qu'il fonctionne avec Isabel. [!INCLUDE[navnow](../../includes/navnow_md.md)] communique au serveur CIS.dll via une fonction wrapper COM.  

Pour configurer votre système afin qu'il fonctionne avec Isabel, suivez les étapes ci-dessous :  

- Installez les composants de sécurité d'Isabel. Pour en savoir plus, consultez la section consacrée au téléchargement sur le [site Web Isabel](http://go.microsoft.com/fwlink/?LinkId=210323).  

- Installez la fonction wrapper COM conçue par l'organisation Isabel. Cette fonction wrapper est incluse dans le package d'Isabel GO 6.20.  

- Enregistrez la fonction wrapper COM sur votre ordinateur. Lors de l'invite de commandes, trouvez le fichier intitulé CIS.dll, puis exécutez la commande **regsvr32 CISComWrapper.dll**.  

## <a name="see-also"></a>Voir aussi  
 [Site Web Isabel](http://go.microsoft.com/fwlink/?LinkId=210323)   
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Comment configurer la banque électronique](how-to-set-up-electronic-banking.md)

