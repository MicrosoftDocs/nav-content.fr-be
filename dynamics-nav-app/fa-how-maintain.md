---
title: "Procédure : conserver des immobilisations"
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
ms.openlocfilehash: 58077a38433a73b981a6f3d05ce7ed106acf32f4
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-maintain-fixed-assets"></a>Procédure : conserver des immobilisations
Les frais de maintenance sont des coûts périodiques de routine engagés pour préserver la valeur des immobilisations. Contrairement aux améliorations de capital, ils n'augmentent pas les valeurs.

Vous pouvez enregistrer et mettre à jour un fichier sur la maintenance et l'entretien des immobilisations afin d'accéder facilement aux enregistrements de maintenance complets des immobilisations. Chaque fois qu'une immobilisation est envoyée en réparation, vous enregistrez toutes les informations importantes, par exemple la date de réparation, le numéro du fournisseur et le numéro de téléphone de l'intervenant. La saisie de la maintenance est effectuée pour chaque immobilisation à partir de la fiche immobilisation.

L'actualisation permet d'ajuster des valeurs en fonction de modifications générales de niveau de prix. Le traitement par lots **Réévaluer immobilisations** permet de recalculer les coûts de maintenance.

## <a name="to-record-maintenance-work-on-a-fixed-asset"></a>Pour enregistrer les travaux de maintenance sur une immobilisation  
Vous pouvez enregistrer chaque tâche de maintenance, telle qu'une visite de service, effectuée pour une immobilisation donnée. Pour cela, utilisez la fenêtre **Saisie de la maintenance**.  

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.  
2. Sélectionnez l'immobilisation pour laquelle vous souhaitez enregistrer la maintenance, puis sélectionnez l'action **Saisie de la maintenance**.
3. Dans la fenêtre **Saisie de la maintenance**, renseignez les champs comme nécessaire. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.  

## <a name="to-post-maintenance-costs-from-a-fixed-asset-gl-journal"></a>Pour valider les coûts de maintenance à partir d'une feuille comptabilisation immobilisation
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Liste des lois d'amortissement**, puis sélectionnez le lien connexe.  
2. Sélectionnez la loi d'amortissement qui est attribuée à une immobilisation, puis sélectionnez l'action **Modifier**.
3. Dans la fenêtre **Fiche loi d'amortissement**, veillez à ce que la case **Maintenance** ne soit pas cochée. Cela garantit que les coûts de maintenance ne sont pas validés en comptabilité.
4. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Feuilles compta. immo.**, puis sélectionnez le lien connexe.  
5. Créez une feuille comptable initiale et complétez les champs, le cas échéant.
6. Dans le champ **Type compta. immo**, sélectionnez **Maintenance**.
7. Sélectionnez l'action **Insérer contrepartie immo.**. Une seconde ligne feuille est créée pour le compte contrepartie qui est configuré pour la validation de la maintenance.

    **Remarque** : l'étape 7 ne fonctionne que si vous avez configuré ce qui suit : dans la fenêtre **Fiche groupe compta. immo.** du groupe de validation de l'immobilisation, le champ **Compte maintenance** contient le compte débit général et le champ **Compte contrepartie maintenance** contient le compte général dans lequel vous souhaitez valider les écritures contrepartie pour réévaluation. Pour en savoir plus, voir la section « Pour configurer des groupes de validation d'immobilisation » dans [Procédure : configurer des informations d'immobilisation générales pour les immobilisations](fa-how-setup-general.md).
8. Sélectionnez l'action **Valider**.

## <a name="to-follow-up-on-fixed-assets-service-visits"></a>Pour effectuer le suivi des visites d'entretien des immobilisations
Vous pouvez imprimer l'état **Maintenance - Service suivant** afin de connaître les immobilisations pour lesquelles vous avez programmé une visite de service. Vous pouvez également utiliser cet état lorsque vous mettez à jour le champ **Date prochain service** des fiches immobilisation.  

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Maintenance - Service suivant**, puis sélectionnez le lien connexe.  
2. Renseignez les champs **Date début** et **Date fin**.  
3. Cliquez sur le bouton **Imprimer** ou **Aperçu**.

## <a name="to-monitor-maintenance-costs"></a>Pour surveiller les coûts de maintenance  
Vous pouvez visualiser les coûts de maintenance lorsque vous consultez les statistiques d'une immobilisation.  

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.
2. Sélectionnez l'immobilisation pour laquelle vous souhaitez afficher les coûts de maintenance, puis sélectionnez l'action **Lois d'amortissement**.
3. Dans la fenêtre **Lois d'amortissement immobilisation**, sélectionnez la loi d'amortissement immobilisation pertinente, puis sélectionnez l'action **Statistiques**.
4. Dans la fenêtre **Statistiques immobilisation**, sélectionnez le champ **Maintenance**.

La fenêtre **Écritures comptables maintenance** s'ouvre, affichant les écritures qui constituent le montant dans le champ **Maintenance**.

## <a name="to-view-or-print-maintenance-costs-for-multiple-fixed-assets"></a>Pour afficher ou imprimer les coûts de maintenance pour plusieurs immobilisations  
Dans l'état **Maintenance - Analyse**, vous pouvez choisir de visualiser la maintenance sur un, deux ou trois codes maintenance pour une date ou une période donnée. Vous pouvez également visualiser soit le total de toutes les immobilisations sélectionnées, soit celui de chaque immobilisation.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Maintenance - Analyse**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins.
3. Cliquez sur le bouton **Imprimer** ou **Aperçu**.

## <a name="to-view-maintenance-ledger-entries"></a>Pour visualiser des écritures comptables maintenance
Vous pouvez également étudier les coûts de maintenance en visualisant les écritures comptables.  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.
2. Sélectionnez l'immobilisation pour laquelle vous souhaitez afficher les écritures comptables, puis sélectionnez l'action **Lois d'amortissement**.
3. Dans la fenêtre **Écritures comptables maintenance**, sélectionnez la loi d'amortissement immobilisation pertinente, puis l'action **Statistiques**.

## <a name="to-view-or-print-maintenance-ledger-entries-for-multiple-fixed-assets"></a>Pour afficher ou imprimer les écritures comptables de maintenance pour plusieurs immobilisations  
Dans l'état **Maintenance - Détails**, vous pouvez afficher ou imprimer les écritures comptables de maintenance pour un ou plusieurs actifs.  

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Maintenance - Détails**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins.
3. Cliquez sur le bouton **Imprimer** ou **Aperçu**.

## <a name="see-also"></a>Voir aussi
[Gérer des immobilisations](fa-manage.md)  
[Configurer des immobilisations](fa-setup.md)  
[Finance](finance-setup.md)  
[Bienvenue dans Dynamics NAV](across-get-started.md)

