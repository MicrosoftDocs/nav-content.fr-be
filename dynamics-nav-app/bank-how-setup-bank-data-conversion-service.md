---
title: "Procédure : configurer le service de conversion de données bancaires"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 801e2abee52ec9804028a797e4f330b5e080549a
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-bank-data-conversion-service"></a>Procédure : configurer le service de conversion de données bancaires
Vous pouvez exporter des lignes paiement à partir de la fenêtre **Feuille paiement** vers un flux de données que vous téléchargez ensuite vers votre banque pour un traitement automatique. Ainsi, vous n'avez pas à effectuer de paiements électroniques individuels. Pour plus d'informations, reportez-vous à [Procédure : exportation de paiements vers un fichier bancaire](payables-how-export-payments-bank-file.md).

Un fournisseur global de services permettant de convertir les informations de paiement dans n'importe quel format de données que votre banque requiert est connecté et prêt à être activé dans Dynamics NAV.

Au lieu du service de flux de la banque Envestnet, vous pouvez également utiliser le service de conversion des données bancaires pour obtenir un fichier de relevé bancaire que vous recevez de votre banque converti en flux de données que vous pouvez importer dans Dynamics NAV. Pour plus d'informations, reportez-vous à [Procédure : lettrage automatique des paiements et rapprochement des comptes bancaires](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Remarque** : Le service de conversion de données bancaires peut fixer une limite imposée du nombre de lignes qui peuvent être exportées dans un fichier. Si cette limite est dépassée, vous recevrez un message d'erreur. Il est conseillé que les fichiers de relevé bancaire ne dépassent pas 1 000 lignes, sans quoi le temps de traitement dans le service conversion données bancaires peut augmenter de façon significative.

## <a name="to-sign-your-company-up-for-the-bank-data-conversion-service"></a>Pour inscrire votre société au service de conversion des données bancaires
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres service conv. données banque**, puis sélectionnez le lien connexe.  
2. La fenêtre **Paramètres service conv. données banque** s'ouvre avec trois champs préremplis avec les URL appropriées du fournisseur du service de conversion de données bancaires.

    **Remarque** : Dans la base de données de démonstration CRONUS International Ltd., les champs Nom d'utilisateur et Mot de passe sont préremplis avec les informations de connexion à la démonstration, que vous remplacerez par les informations réelles de votre société en vous inscrivant au service de conversion de données bancaires.
3. Dans le champ **URL d'inscription**, cliquez sur le bouton de navigateur pour ouvrir la page d'inscription du fournisseur de service.  
4. Dans la page d'inscription du fournisseur de services de données bancaires, entrez le nom de l'utilisateur et le mot de passe de l'abonnement de votre société au service, puis suivez le processus d'inscription comme indiqué par le fournisseur de service.

    Votre société est désormais inscrite au service de conversion des données bancaires. Saisissez maintenant le nom de l'utilisateur et le mot de passe que vous avez spécifiés pour le service dans les champs de configuration associés dans Dynamics NAV.
5. Dans la fenêtre **Paramètres service conv. données banque**, dans le champ **Nom d'utilisateur**, entrez la même valeur que vous avez validée comme nom de connexion dans la page du fournisseur de service au cours de l'étape 4.
6. Dans le champ **Mot de passe**, entrez la même valeur que vous avez saisie dans le champ **Mot de passe** de la page du fournisseur de service au cours de l'étape 4.

## <a name="to-encrypt-your-login-information"></a>Chiffrer les informations de connexion
Il est recommandé de protéger les informations de connexion que vous saisissez dans la fenêtre **Paramètres service conv. données banque**. Vous pouvez chiffrer des données sur le serveur Dynamics NAV en générant de nouvelles clés de chiffrement ou en important des clés existantes que vous activez sur l'instance de serveur Dynamics NAV qui est connectée à la base de données.

1. Dans la fenêtre **Paramètres service conv. données banque**, sélectionnez l'action **Gestion du chiffrement**.
2. Dans la fenêtre **Gestion du chiffrement des données**, activez le chiffrement de vos données.

##<a name="to-view-or-update-the-list-of-currently-supported-bank-data-formats"></a>Pour afficher ou mettre à jour la liste des formats de données bancaires actuellement pris en charge
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres service conv. données banque**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Paramètres service conv. données banque**, sélectionnez l'action **Nom banque - Liste conversions données** pour ouvrir la liste des noms de banques représentant les formats de données bancaires pris en charge par le service de conversion.
3. Sur la page **Nom banque - Liste conversions données**, sélectionnez l'action **Mettre à jour liste noms banque**.

La liste des formats de données bancaires qui sont pris en charge par le service de conversion de données bancaires est désormais mise à jour. Il s'agit de la liste de noms de banques, filtrés par pays/région, que vous pouvez sélectionner dans le champ **Nom banque - Conversion données** de la fenêtre **Fiche compte bancaire**.

**Remarque** : les formats de données bancaires pris en charge sont aussi mis à jour lorsque vous sélectionnez ou entrez une valeur dans le champ **Nom banque - Conversion données** du compte bancaire.

Vous êtes désormais inscrit au service de conversion des données bancaires. Continuez pour refléter les informations de connexion sur chaque compte bancaire qui utilise le service.

## <a name="to-set-up-bank-accounts-to-use-the-bank-data-conversion-service"></a>Pour configurer des comptes bancaires pour utiliser le service de conversion des données bancaires
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Comptes bancaires**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche d'un compte bancaire pour lequel vous exporterez ou importerez des fichiers bancaires à l'aide du service de conversion de données bancaires.
3. Dans le raccourci **Transfert**, dans le champ **Format exportation paiement**, sélectionnez **Service de conversion de données bancaires - Virement** pour configurer l'exportation de paiement.
4. Dans le champ **Nom banque - Conversion données**, entrez ou sélectionnez le nom du format de données bancaires que vous avez utilisé au cours de l'étape 4 dans la section « Pour s'inscrire au service de conversion de données bancaires ».
5. Répétez les étapes 1 à 4 pour les autres comptes bancaires qui utiliseront le service de conversion de données bancaires.

## <a name="see-also"></a>Voir aussi  
[Configuration des opérations bancaires](bank-setup-banking.md)  
[Gérer les comptes bancaires](bank-manage-bank-accounts.md)

