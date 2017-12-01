---
title: "Comment configurer la banque électronique"
description: "Avec la banque électronique, vous pouvez effectuer des paiements électroniques pour des fournisseurs et des clients nationaux, internationaux, SEPA ou SEPA non libellés en Euro."
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
ms.openlocfilehash: 63ddc88627d5c3a9d6692d7e9573617da8aaea30
ms.contentlocale: fr-be
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-electronic-banking"></a>Comment configurer la banque électronique
Avec la banque électronique, vous pouvez effectuer des paiements électroniques pour des fournisseurs et des clients nationaux, internationaux, SEPA ou SEPA non libellés en Euro.  

Votre société souscrit un contrat eBanking avec la banque pour maintenir un certain compte bancaire ou plusieurs comptes bancaires. La société s'inscrit également auprès d'Isabel pour envoyer des fichiers paiement à la banque et recevoir des fichiers relevé bancaire de la banque par voie électronique. La société reçoit ainsi des cartes à puce liées au contrat eBanking. Les cartes à puce sont sécurisées par code PIN.  

Vous recevrez l'une de ces cartes à puce pour vous connecter à IBS et être lié au contrat eBanking de la société.  

Lors du téléchargement de fichiers vers ou depuis la plateforme IBS, vous insérerez la carte à puce dans le lecteur de carte et utiliserez un code PIN pour établir la connexion à IBS. Lorsque la connexion à IBS est établie, le contrat eBanking et l'utilisateur eBanking sont reconnus par le système. Les numéros de compte liés du contrat eBanking et de l'utilisateur sont également reconnus.  

Avant de pouvoir utiliser la banque électronique, vous devez configurer les informations suivantes :  

- Configuration de la banque électronique.  
- Codes IBLC/BLWI : pour plus d'informations, voir [Comment configurer des codes transaction IBLC-BLWI](how-to-set-up-iblc-blwi-transaction-codes.md).  
- Comptes bancaires préférés (facultatif).  

## <a name="to-set-up-electronic-banking"></a>Pour configurer la banque électronique  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Configuration de la banque électronique**, puis sélectionnez le lien correspondant.  
2.  Dans la fenêtre **Configuration de la banque électronique**, dans le raccourci **Général**, remplissez les champs comme indiqué dans le tableau suivant.   

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Résumer lignes FS**|Sélectionnez pour indiquer si vous souhaitez regrouper les lignes feuilles paiement pour chaque fournisseur.|  
    |**Couper comm. de paiement**|Sélectionnez pour indiquer si vous souhaitez tronquer les longues communications de paiement. Les communications seront tronquées si elles contiennent plus de 106 caractères pour les paiements nationaux et plus de 140 caractères pour les paiements internationaux.|  
    |**Version IBS**|Spécifiez la version d'Isabel actuellement utilisée pour la fonction de banque électronique dans votre organisation.|  
    |**Adresse électronique de notification**|Spécifiez l'adresse électronique de notification que vous souhaitez utiliser pour les messages concernant les transactions et le solde de la banque électronique. Il s'agit de l'adresse par défaut utilisée pour contacter le serveur Isabel.|  
    |**Langue**|Spécifiez la langue que vous souhaitez utiliser pour les messages concernant les transactions et le solde de la banque électronique.|  
    |**Version de service IBS**|Spécifiez la version du service utilisée pour communiquer avec le serveur Isabel.|  

3.  Dans le raccourci **Télécharger**, remplissez les champs comme indiqué dans le tableau suivant.   

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Mode d'intégration du téléchargement (amont)**|Spécifiez le mode que vous souhaitez utiliser pour télécharger du contenu sur le serveur Isabel. Les options du mode d'intégration incluent **Interactif** et **Manuel**. Si le mode d'intégration est défini sur **Interactif**, vous devez définir le champ **Version IBS** sur **6**. Les écritures de la table **Journal IBS** seront créées lorsque les fichiers paiement seront générés. Si le mode d'intégration est défini sur **Manuel**, vous devez vous connecter au serveur Isabel manuellement, et aucune écriture ne sera créée.|  
    |**Chemin du téléchargement (amont)**|Spécifiez le chemin d'accès au dossier où les fichiers sont enregistrés au cours du téléchargement sur le serveur.|  

4.  Dans le raccourci **Télécharger**, remplissez les champs comme indiqué dans le tableau suivant.   

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Mode d'intégration du téléchargement (aval)**|Spécifiez le mode que vous souhaitez utiliser pour télécharger du contenu sur le serveur Isabel. Les options incluent **Interactif** et **Manuel**. Si le mode d'intégration est défini sur **Interactif**, vous devez définir le champ **Version IBS** sur **6**. Les écritures de la table **Journal IBS** seront créées à l'issue du téléchargement. Si le mode d'intégration est défini sur **Manuel**, vous devez vous connecter au serveur Isabel manuellement, et aucune écriture ne sera créée.|  
    |**Chemin du téléchargement (aval)**|Spécifiez le chemin d'accès au dossier où les fichiers sont enregistrés au cours du téléchargement depuis le serveur.|  

5.  Dans le raccourci **Numérotation**, remplissez les champs comme indiqué dans le tableau suivant.   

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nos de téléchargement (amont) du journal IBS**|Spécifiez la souche de numéros utilisée pour les écritures journal Isabel qui sont créées au cours du téléchargement sur le serveur.|  
    |**Nos de téléchargement (aval) du journal IBS**|Spécifiez la souche de numéros utilisée pour les écritures journal Isabel qui sont créées au cours du téléchargement des fichiers du serveur.|  
    |**ID demande IBS**|Spécifiez une séquence de numéros utilisée pour la numérotation automatique et unique des demandes.|  

6.  Cliquez sur le bouton **OK**.  

Si vous le souhaitez, vous pouvez attribuer des comptes bancaires à chaque client et à chaque fournisseur. Cela facilite les paiements électroniques. La procédure suivante est consacrée à l'attribution de comptes bancaires préférés aux clients, mais les mêmes instructions s'appliquent aux fournisseurs.  

## <a name="to-add-a-preferred-bank-account-to-a-customer"></a>Pour ajouter un compte bancaire préféré à un client  

1.  Sélectionnez l'icône ![Rechercher une page ou un état](../../media/ui-search/search_small.png "icône Rechercher une page ou un état"), entrez **Clients**, puis sélectionnez le lien correspondant.  
2.  Sélectionnez un client, puis choisissez l'action **Modifier**.  
3.  Dans le raccourci **Paiements**, entrez le **Compte bancaire préféré**, puis cliquez sur le bouton **OK**.  

    > [!NOTE]  
    >  Pour tous les paiements, utilisez un compte bancaire par client ou par fournisseur.  

4.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Site Web Isabel](http://go.microsoft.com/fwlink/?LinkId=210323)   
 [Banque électronique belge](belgian-electronic-banking.md)   
 [Paiements électroniques belges](belgian-electronic-payments.md)   
 [Comment configurer les codes transaction IBLC/BLWI](how-to-set-up-iblc-blwi-transaction-codes.md)   
 [Comment configurer les fournisseurs pour les propositions de paiement automatique](how-to-set-up-vendors-for-automatic-payment-suggestions.md)   
 [Comment générer des propositions de paiement](how-to-generate-payment-suggestions.md)   
 [Comment créer des modèles et lots feuille paiement](how-to-create-payment-journal-templates-and-batches.md)   
 [Comment tester les paiements électroniques](how-to-test-electronic-payments.md)   
 [Comment gérer les lignes paiement électronique](how-to-manage-electronic-payment-lines.md)   
 [Comment imprimer les fichiers paiement](how-to-print-payment-files.md)

