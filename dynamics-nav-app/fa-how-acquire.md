---
title: "Procédure : acquérir des immobilisations"
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
ms.openlocfilehash: 5b58a6cf0a0c22c8076082328f92725cb7dbc4d1
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-acquire-fixed-assets"></a>Procédure : acquérir des immobilisations
Pour chaque immobilisation, vous devez créer une fiche contenant des informations la concernant. Vous pouvez configurer des bâtiments ou un équipement de production en tant qu'actif principal avec une liste de composants et vous pouvez les regrouper de différentes façons, comme par catégorie, département ou emplacement. Une loi d'amortissement doit être configurée et assignée à chaque immobilisation avant que vous puissiez l'acquérir.

Lorsqu'une immobilisation est configurée et lorsqu'une loi d'amortissement est attribuée, vous devez acquérir l'immobilisation. Pour acquérir une immobilisation, vous enregistrez son coût d'acquisition dans le compte général, le compte bancaire ou le fournisseur pertinent en validant une transaction d'acquisition à partir de la fenêtre **Feuille compta. immo.**. Vous pouvez utiliser la fenêtre **Acquisition d'immobilisation assistée** pour créer et valider automatiquement les lignes feuille comptabilité requises.

La valeur résiduelle est la valeur restante d'une immobilisation qui est devenue inutilisable. Vous pouvez valider la valeur résiduelle à partir d'une feuille immobilisation lors de la validation du coût d'acquisition. Pour en savoir plus, voir [Procédure : amortir des immobilisations](fa-how-depreciate-amortize.md).

L'actualisation permet d'ajuster des valeurs en fonction de modifications générales de niveau de prix. Le traitement par lots **Réévaluer immobilisations** permet de calculer les coûts d'acquisition à des coûts de remplacement.

## <a name="to-create-a-fixed-asset-and-acquire-it-automatically"></a>Pour créer une immobilisation et l'acquérir automatiquement
La procédure suivante décrit comment créer une immobilisation, puis l'acquérir via la fenêtre **Acquisition d'immobilisation assistée** pour créer et valider les lignes feuille validation immobilisation requises. Vous pouvez également créer et valider les lignes feuille manuellement. Pour en savoir plus, voir la section « Pour valider manuellement une acquisition d'immobilisation avec la feuille validation immobilisation ».

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.  
2. Sélectionnez l'action **Nouveau**, puis renseignez les champs du raccourci **Général**, le cas échéant. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Sur le raccourci **Loi d'amortissement**, renseignez les champs, le cas échéant. Cette étape attribue une loi d'amortissement à l'immobilisation.  
4. Si vous devez assigner plus d'une loi d'amortissement à l'immobilisation, sélectionnez l'action **Ajouter davantage de lois d'amortissement**. Pour en savoir plus, voir la section « Assigner une loi d'amortissement à une immobilisation » dans [Procédure : définir l'amortissement d'immobilisation](fa-how-setup-depreciation.md).

    Lorsque tous les champs obligatoires pour acquérir une immobilisation sont complétés, la notification **Vous êtes sur le point d'acquérir l'immobilisation. Acquérir** s'affiche en haut de la page.
5. Sélectionnez l'action **Acquérir** dans la notification.
6. Suivez les étapes dans la fenêtre **Acquisition d'immobilisation assistée** pour terminer l'acquisition automatique de l'immobilisation.

**Remarque** : vous pouvez également valider le coût d'acquisition en tant qu'avoirs. Dans ce cas, n'oubliez pas que la valeur du champ **Coût d'acquisition TVA incluse** doit comporter un signe moins pour indiquer un avoir.

Lorsque vous sélectionnez **Terminer**, le champ **Valeur comptable** de la fenêtre **Fiche immobilisation** est renseigné, indiquant que l'immobilisation a été acquise au coût d'acquisition spécifié.  

## <a name="to-set-up-a-component-list-for-a-main-asset"></a>Pour configurer une liste de composants pour une immobilisation principale  
Vous pouvez regrouper les immobilisations en immobilisations principales divisées en composants. Par exemple, si vous disposez d'une machine de production composée de différentes pièces, vous pouvez regrouper ces pièces de cette manière.  

Vous devez définir à la fois l'immobilisation principale et ses composants en tant que fiches immobilisation individuelles. Une fois la liste de composants créée, Dynamics NAV renseigne automatiquement les champs **Immo. principale/Composant** et **Composants immo. principale** sur les fiches immobilisation.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.
2. Sélectionnez l'immobilisation principale, puis l'action **Composants immo. principale**.
3. Dans la fenêtre **Composants immo. principale**, sélectionnez le champ **N° immo**. , puis sélectionnez l'immobilisation que vous souhaitez ajouter en tant que composant de l'immobilisation principale.
4. Fermez la fenêtre.
5. Répétez les étapes 3 et 4 pour chaque composant de l'immobilisation que vous souhaitez ajouter.
6. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres immobilisations**, puis sélectionnez le lien connexe.
7. Cochez la case **Compta. immo. princip.**.

## <a name="to-post-a-fixed-asset-acquisition-manually-with-the-fixed-asset-gl-journal"></a>Pour valider manuellement une acquisition d'immobilisation avec une feuille validation immobilisation
La procédure suivante décrit comment acquérir manuellement une immobilisation en créant et en validant des lignes dans la fenêtre **Feuille compta. immo.**. Vous pouvez également acquérir automatiquement une immobilisation via la fenêtre **Acquisition d'immobilisation assistée**. Pour en savoir plus, voir l'étape 5 de la section « Pour créer une immobilisation et l'acquérir automatiquement ».

**Remarque** : vous pouvez également valider le coût d'acquisition en tant qu'avoirs. Dans ce cas, n'oubliez pas que la valeur du champ **Montant** doit comporter un signe moins pour indiquer un avoir.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Feuilles compta. immo.**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Feuille compta. immo.**, dans le champ **Type compta. immo.**, sélectionnez **Coût acquisition**.
3. Renseignez les champs restants selon vos besoins.
4. Sélectionnez l'action **Valider**.  

**Astuce** : si vous complétez le champ **N° assurance** dans la feuille validation immobilisation lorsque vous validez un coût d'acquisition, Dynamics NAV valide également le coût d'acquisition de l'immobilisation dans les écritures couverture assurance. Pour en savoir plus, voir [Procédure : assurer des immobilisations](fa-how-insure.md).

## <a name="to-cancel-an-acquisition-cost-posting-for-one-fixed-asset"></a>Pour annuler la validation du coût d'une acquisition pour une immobilisation
Si vous faites une erreur lors de la validation d'un coût d'acquisition, vous pouvez supprimer l'écriture à l'aide du traitement par lots **Annuler écritures immo**, puis valider l'écriture d'acquisition correcte. Les écritures erronées sont transférées vers la fenêtre **Erreur écritures comptables immo.**.

Par exemple, si vous validez une acquisition avec une date erronée, vous devez la corriger dès que possible, car la date de validation de l'immobilisation est utilisée dans de nombreux calculs essentiels.

**Important** : vous ne pouvez pas utiliser la fonction **Transaction contre-passée** pour les écritures comptables immobilisation.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Annuler les écritures comptables immobilisation**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Pour lancer le traitement par lots, cliquez sur le bouton **OK**.
4. Lorsqu'une écriture incorrecte ou lorsque plusieurs écritures incorrectes sont annulées, continuez à valider le coût d'acquisition exact.

Pour annuler les écritures comptables pour plusieurs immobilisations à la fois, utilisez le traitement par lots **Annuler les écritures comptables immobilisation**.

## <a name="to-post-the-salvage-value-together-with-the-acquisition-cost"></a>Pour valider la valeur résiduelle ainsi que le coût d'acquisition  
Vous pouvez valider la valeur résiduelle avec le coût d'acquisition à partir d'une feuille comptable immobilisation.    

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Annuler les écritures comptables immobilisation**, puis sélectionnez le lien connexe.
2. Créez la ligne feuille d'acquisition. Pour en savoir plus, voir la section « Pour valider manuellement une acquisition d'immobilisation avec la feuille validation immobilisation ».
3. Dans le champ **Valeur résiduelle** de la ligne feuille, saisissez le montant de la valeur résiduelle comme avoir (avec un signe moins).
4. Sélectionnez l'action **Valider**.

**Remarque** : le type de validation **Valeur résiduelle** est une option disponible uniquement dans la fenêtre **Feuille immo.**. Elle n'est pas disponible dans la fenêtre **Feuille compta. immo.**, car la valeur résiduelle n'est jamais affichée en comptabilité.

## <a name="see-also"></a>Voir aussi
[Gérer des immobilisations](fa-manage.md)  
[Configurer des immobilisations](fa-setup.md)  
[Finance](finance-setup.md)  
[Bienvenue dans Dynamics NAV](across-get-started.md)
