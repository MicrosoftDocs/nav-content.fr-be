---
title: Isabel 6
description: "L'organisation Isabel a développé une plateforme appelée Client Isabel Synchronizer (CIS), qui permet l'intégration sécurisée de [!INCLUDE[navnow](../../includes/navnow_md.md)] avec Isabel. CIS traite les échanges de documents depuis et vers le serveur Isabel."
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
ms.openlocfilehash: 73f14e2c6334b820a22d7834b195493f33c2a426
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

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

