---
title: "Procédure: configurer le service de flux de la Envestnet Yodlee Bank"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 270568214afd2ca8af15f0fa7640337c77ec2f1e
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-envestnet-yodlee-bank-feeds-service"></a>Procédure: configurer le service de flux de la Envestnet Yodlee Bank
Vous pouvez importer des relevés bancaires électroniques auprès de votre banque pour renseigner rapidement la fenêtre **Feuille rapprochement bancaire** de sorte à pouvoir lettrer les paiements et rapprocher le compte bancaire. Pour plus d'informations, reportez-vous à [Lettrage automatique des paiements et rapprochement des comptes bancaires](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Remarque** : le service Envestnet Yodlee Bank Feeds, ou tout service de flux bancaire d'un autre fournisseur, risque de ne pas être disponible dans votre système. Contactez votre partenaire Microsoft si vous souhaitez utiliser un service de flux bancaire pour importer les relevés bancaires.

Une fois que vous avez activé le service de flux bancaire, vous devez lier le compte bancaire concerné au compte bancaire en ligne à partir duquel proviendra le flux. Vous liez des comptes bancaires à des comptes bancaires en ligne dans chacun des scénarios suivants :

- Un compte bancaire n'existe pas dans Dynamics NAV pour votre compte bancaire en ligne. Par conséquent, vous créez le compte bancaire en le liant à partir du compte bancaire en ligne.
- Vous souhaitez lier un compte bancaire existant dans Dynamics NAV à un compte bancaire en ligne.
- Un compte bancaire lié doit être dissocié car vous souhaitez arrêter d'utiliser le service de flux bancaire pour le compte.
- Les comptes bancaires en ligne ont changé et vous souhaitez mettre à jour les informations relatives aux comptes bancaires dans Dynamics NAV.

Lorsque le service de flux bancaire est activé, vous pouvez configurer un compte bancaire de sorte à importer automatiquement de nouveaux relevés bancaires dans la fenêtre **Feuille rapprochement bancaire** toutes les deux heures. Les transactions pour les paiements qui ont déjà été validés comme lettrés et/ou rapprochés dans la fenêtre **Feuille rapprochement bancaire** ne sont pas importées. Pour en savoir plus, voir la section « Pour activer l'importation automatique des relevés bancaires ».

**Remarque** : si vous utilisez la configuration assistée Configurer la société, certaines étapes des procédures suivantes sont effectuées automatiquement lorsque vous parvenez à la configuration de compte bancaire de la société. Pour en savoir plus, voir [Bienvenue dans Dynamics NAV](across-get-started.md).

## <a name="to-enable-the-bank-feed-service"></a>Pour activer le service de flux bancaire
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Comptes bancaires**, puis sélectionnez le lien connexe.
2. Ouvrez le compte bancaire que vous allez utiliser pour le service de flux bancaire.
3. Dans la fenêtre **Compte bancaire**, dans le champ **Format importation relevé bancaire**, sélectionnez YODLEEBANKFEED.  

Le service de flux bancaire est activé lorsque vous liez un compte bancaire à son compte bancaire en ligne connexe. Consultez la procédure suivante.  

## <a name="to-create-a-new-linked-bank-account"></a>Pour créer un compte bancaire lié
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Comptes bancaires**, puis sélectionnez le lien connexe.
2. Sélectionnez le compte bancaire approprié, puis sélectionnez **Créer un compte bancaire lié**. La fenêtre **Comptes bancaires liés** s'ouvre au bout de quelques instants.

    **Remarque** : cette fenêtre affiche la page Web réelle du service de flux de la Envestnet Yodlee Bank. La terminologie et la fonctionnalité de la fenêtre peuvent ne pas correspondre aux instructions fournies dans cette rubrique.  
3. Dans la fenêtre **Comptes bancaires en ligne liés**, dans le volet **Lier un compte**, utilisez la fonction de recherche pour trouver la banque qui abrite un ou plusieurs de vos comptes bancaires en ligne.
4. Choisissez le nom de la banque. Le volet **Connexion** s'ouvre.
5. Saisissez le nom de l'utilisateur et le mot de passe que vous utilisez pour la connexion à la banque en ligne, puis cliquez sur le bouton **Suivant**.  
6. Le service de flux bancaire se prépare à rattacher le premier compte bancaire en ligne de la banque spécifiée à un nouveau compte bancaire dans Dynamics NAV.

    **Remarque** : si vous disposez de plusieurs comptes bancaires en ligne dans cette banque, vous devez créer des comptes bancaires supplémentaires pour ceux-ci dans Dynamics NAV. Voir les étapes 8 à 10.

    Une fois le processus accompli, le nom de la banque s'affiche dans le volet **Mes comptes** de l'onglet **Lié**. Le numéro entre parenthèses indique le nombre de comptes bancaires en ligne ayant été liés.
7. Cliquez sur le bouton **OK**.

    Si un seul compte bancaire en ligne est lié la fenêtre **Fiche compte bancaire** pour un nouveau compte bancaire s'ouvre, préremplie avec le nom du compte bancaire en ligne. Dans ce cas, la tâche de liaison de compte bancaire est terminée. Il ne vous reste plus qu'à configurer le compte bancaire. Pour plus d'informations, reportez vous à [Procédure: configuration de comptes bancaires](bank-how-setup-bank-accounts.md).

    Si plusieurs comptes bancaires en ligne ont été rattachés, la fenêtre **Comptes bancaires liés** s'ouvre et répertorie les comptes bancaires en ligne supplémentaires qui n'ont pas encore été rattachés à des comptes bancaires dans Dynamics NAV. Dans ce cas, suivez l'étape suivante.  
8. Dans la fenêtre **Comptes bancaires liés**, sélectionnez la ligne correspondant à un compte bancaire en ligne, puis sélectionnez l'action **Lier à un nouveau compte bancaire**.

    La fenêtre **Fiche compte bancaire** pour un nouveau compte bancaire s'ouvre, préremplie avec le nom du compte bancaire en ligne.

    Si un compte bancaire existe déjà dans Dynamics NAV auquel vous souhaitez lier le compte bancaire en ligne supplémentaire, procédez comme suit.  
9. Dans la fenêtre **Comptes bancaires liés**, sélectionnez la ligne correspondant à un compte bancaire en ligne, puis sélectionnez l'action **Lier à un compte bancaire existant**.
10. Dans la fenêtre **Liste des comptes bancaires**, sélectionnez le compte bancaire que vous voulez lier, puis cliquez sur le bouton **OK**.

## <a name="to-link-a-bank-account-to-an-online-bank-account"></a>Pour lier un compte bancaire à un compte bancaire en ligne
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Comptes bancaires**, puis sélectionnez le lien connexe.
2. Sélectionnez la ligne correspondant à un compte bancaire qui n'est pas lié à un compte bancaire en ligne, puis sélectionnez l'action **Lier au compte bancaire en ligne**. La fenêtre **Comptes bancaires en ligne liés** s'ouvre, préremplie avec le nom de la banque dans le volet **Lier un compte**.
3. Choisissez le nom de la banque. Le volet **Connexion** s'ouvre.
4. Saisissez le nom de l'utilisateur et le mot de passe que vous utilisez pour la connexion à la banque en ligne, puis cliquez sur le bouton **Suivant**.

    Le service de flux bancaire se prépare à lier votre compte bancaire de Dynamics NAV au compte bancaire en ligne connexe.

    Une fois le processus accompli, le nom de la banque s'affiche dans le volet **Mes comptes** de l'onglet **Lié**. Si la banque a plus d'un compte bancaire, seul le compte bancaire que vous avez sélectionné au cours de l'étape 2 est lié.
5. Cliquez sur le bouton **OK**.

Dans la fenêtre **Liste des comptes bancaires**, la case **Lié** est cochée.

## <a name="to-unlink-a-bank-account"></a>Pour détacher un compte bancaire en ligne
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Comptes bancaires**, puis sélectionnez le lien connexe.  
2. Sélectionnez la ligne correspondant à un compte bancaire lié que vous souhaitez détacher du compte bancaire en ligne connexe, puis sélectionnez l'action **Détacher le compte bancaire en ligne**.

**Remarque** : si vous choisissez **Oui** dans la boîte de dialogue de confirmation, le lien vers le compte bancaire en ligne est supprimé, et les informations de connexion sont effacées. Pour lier à nouveau le compte bancaire au compte bancaire en ligne, vous devez vous connecter de nouveau à la banque. Pour en savoir plus, voir la section « Pour lier un compte bancaire à un compte bancaire en ligne ».

## <a name="to-update-bank-account-linking"></a>Pour mettre à jour la liaison des comptes bancaires
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Comptes bancaires**, puis sélectionnez le lien connexe.
2. Sélectionnez le compte bancaire approprié, puis sélectionnez l'action **Mettre à jour la liaison des comptes bancaires**.

Si des problèmes existent pour les comptes bancaires liés dans la fenêtre **Liste des comptes bancaires**, la fenêtre **Comptes bancaires liés** s'ouvre et indique les comptes bancaires affectés par des problèmes. Le meilleur moyen de résoudre ces problèmes est de détacher le compte bancaire en ligne, puis de recréer le lien. Pour en savoir plus, voir la section « Pour lier un compte bancaire à un compte bancaire en ligne ».

## <a name="to-enable-automatic-import-of-bank-statements"></a>Pour activer l'importation automatique des relevés bancaires
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Comptes bancaires**, puis sélectionnez le lien connexe.
2. Sélectionnez la ligne correspondant à un compte bancaire lié, puis sélectionnez l'action **Configuration de l'importation de relevés bancaires automatique**.
3. Dans la fenêtre **Configuration de l'importation de relevés bancaires automatique**, dans le champ **Nombre de jours inclus**, indiquez jusqu'à quelle date il faut remonter dans le temps pour obtenir les nouvelles transactions bancaires.

    **Remarque** : il est recommandé de définir cette valeur à 7 jours ou plus.
4. Cochez la case **Activé**.  
Toutes les heures, la fenêtre **Feuille rapprochement bancaire** sera renseignée avec tous les nouveaux paiements effectués sur le compte bancaire en ligne.

**Remarque** : les transactions pour les paiements qui ont déjà été validés comme lettrés et/ou rapprochés dans la fenêtre **Feuille rapprochement bancaire** ne sont pas importées.

## <a name="see-also"></a>Voir aussi  
[Configuration des opérations bancaires](bank-setup-banking.md)  
[Gérer les comptes bancaires](bank-manage-bank-accounts.md)  
[Procédure : lettrage automatique des paiements et rapprochement des comptes bancaires](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Personnalisation de Dynamics NAV à l'aide des extensions ](ui-extensions.md)

