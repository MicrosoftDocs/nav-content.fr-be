---
title: "Méthodes d'amortissement"
description: "En savoir plus sur les différentes méthodes pour amortir ou déprécier des immobilisations."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: write down
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7d5fd80eeabb078122283748c45203356bf6f1a8
ms.contentlocale: fr-be
ms.lasthandoff: 10/16/2017

---
# <a name="depreciation-methods"></a>Méthodes d'amortissement
Huit méthodes d'amortissement sont disponibles :  

* Linéaire  
* Dégressif1  
* Dégressif2  
* Dégr1/Lin  
* Dégr2/Lin  
* Paramétrable  
* Manuel  

  > [!NOTE]  
>   Utilisez cette méthode pour les immobilisations qui ne font pas l'objet d'un amortissement, par exemple les terrains. Vous devez saisir l'amortissement dans la feuille validation immobilisation. Le traitement par lots **Calculer amortissement** ignore les immobilisations qui utilisent cette méthode d'amortissement.  
* Règle de la demi-année  

  > [!NOTE]  
>    Lorsque vous utilisez cette méthode, le montant de l'amortissement d'une immobilisation ne varie pas d'une année à l'autre.  

## <a name="straight-line-depreciation"></a>Amortissement linéaire
Lorsque vous utilisez la méthode linéaire, vous devez indiquer l'une des options suivantes dans la loi d'amortissement immobilisation :  

* Période de l'amortissement (en années ou en mois) ou date fin de l'amortissement  
* Pourcentage annuel fixe  
* Montant annuel fixe  
* Période d'amortissement  

### <a name="depreciation-period"></a>Période d'amortissement
Si vous saisissez la période d'amortissement (nombre d'années ou de mois d'amortissement, ou date fin d'amortissement), la formule suivante calcule le montant de l'amortissement :  

*Montant de l'amortissement = ((valeur comptable - valeur résiduelle) x nombre de jours d'amortissement)/jours d'amortissement restants*  

Le nombre de jours d'amortissement restants correspond au nombre de jours d'amortissement moins le nombre de jours compris entre la date début de l'amortissement et la date de la dernière écriture immobilisation.  

La valeur comptable peut être diminuée d'un montant de réévaluation, de dépréciation, ou paramétrable 1 ou 2 validé, selon l'état (activé/désactivé) des champs **Inclure dans calcul amort.** et **Elément valeur comptable** dans la fenêtre **Type paramètre compta. immo.**. Ce calcul garantit l'amortissement complet de l'immobilisation à la date fin de l'amortissement.  

### <a name="fixed-yearly-percentage"></a>Pourcentage annuel fixe
Si vous saisissez un pourcentage annuel fixe, le programme utilise la formule suivante pour calculer le montant de l'amortissement :  

Montant de l'amortissement = (% linéaire x base amortissement x nombre de jours d'amortissement)/(100 x 360)  

### <a name="fixed-yearly-amount"></a>Montant annuel fixe
Si vous saisissez un montant annuel fixe, le programme utilise la formule suivante pour calculer le montant de l'amortissement :  

Montant de l'amortissement = (montant d'amortissement fixe x nombre de jours d'amortissement)/360  

### <a name="example---straight-line-depreciation"></a>Exemple - Amortissement linéaire
Une immobilisation a un coût d'acquisition de 100 000 DS. Sa durée de vie est estimée à huit ans. Le traitement par lots **Calculer amortissement** est exécuté tous les semestres.  

Pour cet exemple, l'écriture comptable immobilisation se présente comme suit :  

| Date | Type compta. immo. | Jours | Montant | Valeur comptable |
| --- | --- | --- | --- | --- |
| 01/01/10 |Coût acquisition |* |10 000,00 |10 000,00 |
| 30/06/10 |Amortissements |180 |-6 250,00 |93,750.00 |
| 31/12/10 |Amortissements |180 |-6 250,00 |87,500.00 |
| 30/06/11 |Amortissements |180 |-6 250,00 |81,250.00 |
| 31/12/11 |Amortissements |180 |-6 250,00 |75,000.00 |
| 30/06/17 |Amortissements |180 |-6 250,00 |6,250.00 |
| 31/12/17 |Amortissements |180 |-6 250,00 |0 |

* Date début amortissement  

## <a name="declining-balance-1-depreciation"></a>Amortissement dégressif 1
Il s'agit d'une méthode d'amortissement accélérée qui ventile la plus grande portion du coût d'une immobilisation sur les premières années de sa durée de vie. Si vous utilisez cette méthode, vous devez saisir un pourcentage annuel fixe.  

La formule suivante calcule les montants d'amortissement :  

*Montant de l'amortissement = (% dégressif x nombre de jours d'amortissement x base amortissement)/(100 x 360)*  

La base d'amortissement correspond à la valeur comptable moins l'amortissement validé depuis la date début de l'exercice comptable en cours.  

Le montant de l'amortissement validé peut contenir des écritures avec divers types de validation (dépréciation, paramétrable 1 et paramétrable 2) validés depuis la date de début de l'exercice comptable en cours. Ces types de validation sont inclus dans le montant d'amortissement validé si vous avez coché les champs **Type amortissement** et **Elément valeur comptable** dans la fenêtre **Type paramètre compta. immo.**.  

### <a name="example---declining-balance-1-depreciation"></a>Exemple - Amortissement dégressif 1
Une immobilisation a un coût d'acquisition de 100 000 DS. Le champ **% dégressif** indique la valeur 25. Le traitement par lots **Calculer amortissement** est exécuté tous les semestres.  

Le tableau suivant montre à quoi ressemblent les écritures comptables immobilisation.  

| Date | Type compta. immo. | Jours | Montant | Valeur comptable |
| --- | --- | --- | --- | --- |
| 01/01/10 |Coûts d'acquisition |* |10 000,00 |10 000,00 |
| 30/06/10 |Amortissements |180 |-12 500,00 |87,500.00 |
| 31/12/10 |Amortissements |180 |-12 500,00 |75,000.00 |
| 30/06/11 |Amortissements |180 |-9 375,00 |65,625.00 |
| 31/12/11 |Amortissements |180 |-9 375,00 |56,250.00 |
| 30/06/12 |Amortissements |180 |-7 031,25 |49,218.75 |
| 31/12/12 |Amortissements |180 |-7 031,25 |42,187.50 |
| 30/06/13 |Amortissements |180 |-5 273,44 |36,914.06 |
| 31/12/13 |Amortissements |180 |-5 273,44 |31,640.62 |
| 30/06/14 |Amortissements |180 |-3 955,08 |27,685.54 |
| 31/12/14 |Amortissements |180 |-3 955,08 |23,730.46 |

* Date début amortissement  

    Méthode de calcul :  

    *1ère année : 25 % de 100 000 = 25 000 = 12 500 +12 500*

    *2ème année : 25 % de 75 000 = 18 750 = 9 375 +9 375*

    *3ème année : 25 % de 56 250 = 14 062,50 = 7 031,25 +7 031,25*

    Le calcul continue jusqu'à ce que la valeur comptable soit égale à la valeur résiduelle ou au montant final arrondi que vous avez saisi.   

## <a name="declining-balance-2-depreciation"></a>Amortissement dégressif 2
Les méthodes Dégressif 1 et Dégressif 2 calculent le même montant d'amortissement total chaque année. Toutefois, si vous lancez le traitement par lots **Calculer amortissement** plusieurs fois par an, la méthode Dégressif 1 permet d'obtenir des montants d'amortissement équitables pour chaque période d'amortissement. En revanche, la méthode Dégressif 2 permet d'obtenir des montants d'amortissement qui sont dégressifs pour chaque période.  

### <a name="example---declining-balance-2-depreciation"></a>Exemple - Amortissement dégressif 2
Une immobilisation a un coût d'acquisition de 100 000 DS. Le champ **% dégressif** indique la valeur 25. Le traitement par lots **Calculer amortissement** est exécuté tous les semestres. Les écritures comptables immobilisation se présentent comme suit :  

| Date | Type compta. immo. | Jours | Montant | Valeur comptable |
| --- | --- | --- | --- | --- |
| 01/01/10 |Coûts d'acquisition |* |10 000,00 |10 000,00 |
| 30/06/10 |Amortissements |180 |-13 397,46 |86,602.54 |
| 31/12/10 |Amortissements |180 |-11 602,54 |75,000.00 |
| 30/06/11 |Amortissements |180 |-10 048,09 |64,951.91 |
| 31/12/11 |Amortissements |180 |-8 701,91 |56,250.00 |

* Date début amortissement  

Méthode de calcul :  

* VC = Valeur comptable  
* NJ = Nombre de jours d'amortissement  
* PD = Pourcentage dégressif  
* P = PD/100  
* J = NJ/360  

La formule de calcul des montants d'amortissement est la suivante :  

*MA = VC x (1 - (1 - P)<sup>D<sup>*  

Les valeurs d'amortissement sont les suivantes :  

| Date | Calcul |
| --- | --- |
| 30/06/10 |MA = 100 000,00 (1 - (1 - 0,25)<sup> 0,5<sup>) = 13 397,46 |
| 31/12/10 |MA = 86 602,54 x (1 - (1 - 0,25)<sup> 0,5<sup>) = 11 602,54 |
| 30/06/11 |MA = 75 000,00 x (1 - (1 - 0,25)<sup> 0,5<sup>) = 10 048,09 |
| 31/12/11 |MA = 64 951,91 x (1 - (1 - 0,25)<sup> 0,5<sup>) = 8 701,91 |

## <a name="db1sl-depreciation"></a>Amortissement Dégr1/Lin
Dégr1/Lin est l'abréviation combinée de Dégressif 1 et de Linéaire. Le calcul continue jusqu'à ce que la valeur comptable soit égale à la valeur résiduelle ou au montant final arrondi que vous avez saisi.  

Le traitement par lots **Calculer amortissement** calcule un montant linéaire et un montant dégressif, mais seul le montant le plus élevé des deux est transmis à la feuille.  

Vous pouvez utiliser divers pourcentages pour calculer le montant dégressif.  

Si vous utilisez cette méthode, saisissez la durée de vie estimée et un pourcentage dégressif dans la fenêtre **Loi d'amortissement**.  

### <a name="example---db1-sl-depreciation"></a>Exemple - Amortissement Dégr1/Lin
Une immobilisation a un coût d'acquisition de 100 000 DS. Dans la fenêtre **Loi d'amortissement**, le champ **% dégressif** indique la valeur 25 et le champ **Nombre années amortissement** indique la valeur 8. Le traitement par lots **Calculer amortissement** est exécuté tous les semestres.  

Les écritures comptables immobilisation se présentent comme suit :  

| Date | Type compta. immo. | Jours | Montant | Valeur comptable |
| --- | --- | --- | --- | --- |
| 01/01/10 |Coûts d'acquisition |* |10 000,00 |10 000,00 |
| 30/06/10 |Amortissements |180 |-12 500,00 |87,500.00 |
| 31/12/10 |Amortissements |180 |-12 500,00 |75,000.00 |
| 30/06/11 |Amortissements |180 |-9 375,00 |65,625.00 |
| 31/12/11 |Amortissements |180 |-9 375,00 |56,250.00 |
| 30/06/12 |Amortissements |180 |-7 031,25 |49,218.75 |
| 31/12/12 |Amortissements |180 |-7 031,25 |42,187.50 |
| 30/06/13 |Amortissements |180 |-5 273,44 |36,914.06 |
| 31/12/13 |Amortissements |180 |-5 273,44 |31,640.62 |
| 30/06/14 |Amortissements |180 |-3 955,08 |27,685.54 |
| 31/12/14 |Amortissements |180 |-3 955,08 |23,730.46 |
| 30/06/15 |Amortissements |180 |-3 955,08 |19.775,38 Lin. |
| 31/12/15 |Amortissements |180 |-3 955,08 |15.820,30 Lin. |
| 30/06/16 |Amortissements |180 |-3 955,08 |11.865,22 Lin. |
| 31/12/16 |Amortissements |180 |-3 955,07 |7.910,15 Lin. |
| 30/06/17 |Amortissements |180 |-3 955,08 |3.955,07 Lin. |
| 31/12/17 |Amortissements |180 |-3 955,07 |0,00 Lin. |

* Date début amortissement  

La mention « SL » qui suit la valeur comptable indique que la méthode linéaire a été utilisée.  

Méthode de calcul :  

1ère année :  

*Montant dégressif : 25 % de 100 000 = 25 000 = 12 500 + 12 500*  

*Montant linéaire = 100 000/8 = 12 500 = 6 250 + 6 250*  

Le montant dégressif est utilisé car il s'agit de la valeur la plus élevée.  

6ème année (2015) :  

*Montant dégressif : 25 % de 23 730,46 = 4 943,85 = 2 471,92 + 2 471,92*  

*Montant linéaire = 23 730,46/3 = 7 910,15 = 3 995,07 + 3 995,08*  

Le montant linéaire est utilisé car il s'agit de la valeur la plus élevée.  

## <a name="user-defined-depreciation"></a>Amortissement défini par l’utilisateur
Le programme dispose d'une option qui vous permet de définir des méthodes d'amortissement paramétrables.  

Avec une méthode paramétrable, vous utilisez la fenêtre **Tables d'amortissement** dans laquelle vous devez saisir un pourcentage d'amortissement pour chaque période (mois, trimestre, année ou période comptable).  

La formule de calcul des montants d'amortissement est la suivante :  

Montant de l'amortissement = (% amortissement x nombre de jours d'amortissement x base amortissement)/(100 x 360)  

### <a name="depreciation-based-on-number-of-units"></a>Amortissement basé sur un nombre d'unités
Cette méthode paramétrable peut également être utilisée pour calculer un amortissement sur la base d'un nombre d'unités, par exemple dans le cas de machines de production dont la durée de vie est préétablie. Dans la fenêtre **Tables d'amortissement**, vous saisissez le nombre d'unités pouvant être produites au cours de chaque période (mois, trimestre, année ou période comptable).  

### <a name="to-set-up-user-defined-depreciation-methods"></a>Pour définir des méthodes d'amortissement paramétrables
Dans la fenêtre **Table amortissement**, vous pouvez configurer des méthodes d'amortissement paramétrables. Par exemple, vous pouvez définir l'amortissement en fonction du nombre d'unités.  

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), saisissez **Tables d'amortissement**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Liste des tables amortissement**, sélectionnez l'action **Nouveau**.  
3. Dans la fenêtre **Fiche table amortissement**, renseignez les champs comme nécessaire. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

### <a name="example---user-defined-depreciation"></a>Exemple - Amortissement défini par l'utilisateur
Vous souhaitez utiliser une méthode d'amortissement vous permettant d'amortir des immobilisations de manière accélérée dans le cadre de l'impôt sur le revenu.  

Pour le calcul de l'impôt, utilisez les taux d'amortissement suivants pour une immobilisation ayant une durée de vie de trois ans :  

* Année 1 : 25%  
* Année 2 : 38%  
* Année 3 : 37%  

Le coût d'acquisition est de 100 000 DS et la durée d'amortissement est de cinq ans. L'amortissement est calculé tous les ans.  

| Date | Type compta. immo. | Jours | Montant | Valeur comptable |
| --- | --- | --- | --- | --- |
| 01/01/10 |Coût acquisition |* |10 000,00 |10 000,00 |
| 31/12/10 |Amortissements |360 |-25 000,00 |75,000.00 |
| 31/12/11 |Amortissements |360 |-38 000,00 |37,000.00 |
| 31/12/12 |Amortissements |360 |-37 000,00 |0 |
| 31/12/13 |Amortissements |Aucun |Aucun |0 |
| 31/12/14 |Amortissements |Aucun |Aucun |0 |

* Date début amortissement  

Si vous utilisez une méthode paramétrable, les champs **Date premier amortissement** et **Date début amortissement** doivent être renseignés dans la fenêtre **Lois d'amortissement immo.** Le champ **Date premier amortissement** et le contenu du champ **Base période** dans la fenêtre **Tables d'amortissement** permettent de déterminer les intervalles de temps à utiliser pour le calcul de l'amortissement. Cela garantit que le programme commence à l'aide du pourcentage spécifié le même jour pour toutes les immobilisations. Le champ **Date début amortissement** permet de calculer le nombre de jours d'amortissement.  

Dans l'exemple précédent, les champs **Date premier amortissement** et **Date début amortissement** indiquent tous les deux la date du 01/01/01. Toutefois, en supposant que le champ **Date premier amortissement** contienne la date 01/01/10 et que le champ **Date début amortissement** indique la valeur 01/04/11, le résultat serait le suivant :  

| Date | Type compta. immo. | Jours | Montant | Valeur comptable |
| --- | --- | --- | --- | --- |
| 01/01/10 |Coût acquisition |* |10 000,00 |10 000,00 |
| 31/12/10 |Amortissements |270 |-18 750,00 |81,250.00 |
| 31/12/11 |Amortissements |360 |-38 000,00 |42,250.00 |
| 31/12/12 |Amortissements |360 |-37 000,00 |6,250.00 |
| 31/12/13 |Amortissements |90 |-6 250,00 |0 |
| 31/12/14 |Amortissements |Aucun |Aucun |0 |

* Date début amortissement  

## <a name="half-year-convention-depreciation"></a>Amortissement selon la règle de la demi-année
La règle de la demi-année n'est appliquée que si vous avez coché le champ **Utiliser règle demi-année** dans la fenêtre **Plan amortissement**.  

Cette méthode d'amortissement peut être utilisée en combinaison avec les méthodes d'amortissement suivantes :  

* Linéaire  
* Dégressif1  
* Dégr1/Lin  

Lorsque vous appliquez la règle de la demi-année, une immobilisation a un amortissement de six mois lors du premier exercice comptable, quelle que soit la valeur du champ **Date début amortissement**.  

> [!NOTE]  
>   Avec la règle de la demi-année, la durée de vie restante estimée pour l'immobilisation à la fin de l'exercice comptable indique toujours une demi-année. Par conséquent, pour que la méthode Utiliser règle de la demi-année soit appliquée correctement, le champ **Date fin amortissement** de la fenêtre **Plan amortissement** doit toujours contenir une date antérieure de six mois à la date fin de l'exercice comptable au cours duquel l'immobilisation sera complètement amortie.  

### <a name="example---half-year-convention-depreciation"></a>Exemple - Amortissement selon la règle de la demi-année
Une immobilisation a un coût d'acquisition de 100 000 DS. Le champ **Date début amortissement** indique la valeur 01/03/10. La durée de vie est estimée à cinq ans, ce qui implique que le champ **Date fin amortissement** doit impérativement être paramétré sur la valeur 30/06/15. Le traitement par lots **Calculer amortissement** est exécuté tous les ans. Cet exemple est basé sur un exercice comptable.  

Les écritures comptables immobilisation se présentent comme suit :  

| Date | Type compta. immo. | Jours | Montant | Valeur comptable |
| --- | --- | --- | --- | --- |
| 01/03/10 |Coût acquisition |* |10 000,00 |10 000,00 |
| 31/12/10 |Amortissements |270 |-10 000,00 |90,000.00 |
| 31/12/11 |Amortissements |360 |-20 000,00 |70,000.00 |
| 31/12/12 |Amortissements |360 |-20 000,00 |50,000.00 |
| 31/12/13 |Amortissements |360 |-20 000,00 |30,000.00 |
| 31/12/14 |Amortissements |360 |-20 000,00 |10,000.00 |
| 31/12/15 |Amortissements |180 |-10 000,00 |0.00 |

* Date début amortissement  

## <a name="example---db1sl-depreciation-using-half-year-convention"></a>Exemple - Amortissement dégressif 1/linéaire selon la règle de la demi-année
Une immobilisation a un coût d'acquisition de 100 000 DS. Le champ **Date début amortissement** indique la valeur 01/11/10. La durée de vie est estimée à cinq ans, ce qui implique que le champ **Date fin amortissement** doit impérativement être paramétré sur la valeur 30/06/15. Dans la fenêtre **Loi d'amortissement**, le champ **% dégressif** indique la valeur 40. Le traitement par lots **Calculer amortissement** est exécuté tous les ans. Cet exemple est basé sur un exercice comptable.  

Les écritures comptables immobilisation se présentent comme suit :  

| Date | Type compta. immo. | Jours | Montant | Valeur comptable |
| --- | --- | --- | --- | --- |
| 01/11/10 |Coût acquisition |* |10 000,00 |10 000,00 |
| 31/12/10 |Amortissements |60 |-20 000,00 |80,000.00 |
| 31/12/11 |Amortissements |360 |-32 000,00 |48,000.00 |
| 31/12/12 |Amortissements |360 |-19 200,00 |28,800.00 |
| 31/12/13 |Amortissements |360 |-11 520,00 |17,280.00 |
| 31/12/14 |Amortissements |360 |-11 520,00 |5.760,00 Lin. |
| 31/12/15 |Amortissements |180 |  -5 760,00 |0,00 Lin. |

* Date début amortissement  

La mention « SL » qui suit la valeur comptable indique que la méthode linéaire a été utilisée.  

Méthode de calcul :  

1ère année :  

*Montant dégressif = Montant total année = 40 % de 100 000 = 40 000, soit pour une demi-année 40 000 / 2 = 20 000*  

*Montant linéaire = Montant total année = 100 000 / 5 = 20 000, soit pour une demi-année 20 000 / 2 = 10 000*  

Le montant dégressif est utilisé car il s'agit de la valeur la plus élevée.  

5ème année (2004) :  

*Montant dégressif = 40 % de 17 280,00 = 6 912,00*  

*Montant linéaire = 28 800 / 1,5 = 11 520,00*  

Le montant linéaire est utilisé car il s'agit de la valeur la plus élevée.  

## <a name="duplicating-entries-to-more-depreciation-books"></a>Duplication des écritures dans davantage de lois d'amortissement
Si vous disposez de trois lois d'amortissement, A1, A2 et A3, et que vous souhaitiez dupliquer des écritures de A1 vers A2 et A3, vous pouvez activer le champ **Inclure dans liste duplication** sur les fiches loi d'amortissement de A2 et de A3. Cela peut être utile si la loi d'amortissement A1 est intégrée en comptabilité et utilise la feuille validation immobilisation, et si les lois d'amortissement A2 et A3 ne sont pas intégrées en comptabilité et utilisent la feuille immobilisation.  

Lorsque vous saisissez une écriture pour A1 dans la feuille validation immobilisation et sélectionnez le champ **Utiliser liste duplication**, le programme duplique l'écriture pour les lois A2 et A3 dans la feuille immobilisation lors de la validation de l'écriture.  

> [!NOTE]  
>   Vous ne pouvez pas utiliser la feuille d'origine comme destination de la duplication. Si vous validez des écritures dans la feuille validation immobilisation, vous pouvez les dupliquer dans la feuille immobilisation ou dans la feuille validation immobilisation en utilisant une autre feuille.  

> [!NOTE]  
>   Vous ne pouvez pas utiliser la même souche de numéros dans la feuille validation immobilisation et la feuille immobilisation. Lorsque vous validez des écritures dans la feuille validation immobilisation, vous devez laisser le champ **N° document** vide. Si vous saisissez un numéro dans le champ, il est copié dans la feuille immobilisation. Vous devez modifier manuellement le numéro de document avant de pouvoir valider la feuille.  

## <a name="see-also"></a>Voir aussi
[Immobilisations](fa-manage.md)  
[Paramétrage d'immobilisations](fa-setup.md)  
[Finances](finance.md)  
[Bienvenue dans [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

