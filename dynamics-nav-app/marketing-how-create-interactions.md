---
title: "Procédure : créer des interactions sur les contacts et les segments"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 459a86ad9674e0d61b045743cbcc99ffdb5cacd9
ms.contentlocale: fr-be
ms.lasthandoff: 06/26/2017

---
# <a name="how-to-create-interactions-on-contacts-and-segments"></a>Procédure : créer des interactions sur les contacts et les segments
Vous pouvez créer des interactions pour enregistrer toutes les interactions et toutes les communications que vous entretenez avec vos contacts et segments, par exemple le courrier direct.

Pour pouvoir créer des interactions, vous devez configurer des modèles interaction. Pour plus d'informations, reportez vous à [Configurer des modèles interaction](marketing-interactions.md#set-up-interaction-templates).

## <a name="to-create-an-interaction"></a>Pour créer une interaction
1. Ouvrez le contact, le vendeur, ou l'écriture journal interaction.
2. Sélectionnez l'action **Créer interaction**.
3. Renseignez les champs, puis cliquez sur le bouton **OK**.

**Remarque** : si vous devez effectuer une autre tâche avant de terminer l'interaction, vous pouvez cliquer sur **Annuler** et choisir de terminer l'interaction à une date ultérieure. Cela permet de reporter l'interaction à plus tard.

## <a name="to-finish-and-delete-postponed-interactions"></a>Pour terminer et supprimer les interactions reportées
1. Ouvrez le contact, le vendeur, ou l'écriture journal interaction.
2. Sélectionnez **Interactions reportées**.
3. Sélectionnez l'interaction que vous souhaitez terminer, puis sélectionnez l'action **Reprendre**.

## <a name="to-create-an-interaction-on-a-segment"></a>Pour créer une interaction sur un segment
1. Sur la page d'accueil, sélectionnez **Segments actifs**. Sinon, dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Segments**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Segment**, dans la section **Interaction**, renseignez les champs pour définir l'interaction à affecter au segment.

  Après avoir affecté une interaction au segment, vous pouvez personnaliser l'interaction pour chaque contact au sein du segment, par exemple en sélectionnant un autre modèle interaction sur les lignes de la fenêtre **Segment**.
3. Pour journaliser le segment et les interactions, sélectionnez l'action **Journal**. La fenêtre **Journaliser segment** s’affiche.
4. Si vous souhaitez créer un segment contenant les mêmes contacts, activez la case à cocher **Créer suivi segment**. Pour créer un suivi segment, vous devez avoir indiqué une souche de numéros pour les segments dans la fenêtre **Paramètres Marketing**.

Une interaction est enregistrée pour chaque contact inclus dans le segment dans la table **Ecriture journal interaction**, et le segment est journalisé. Vous pouvez consulter les segments journalisés dans la fenêtre **Segments journalisés**.

Si vous avez activé la case à cocher **Créer suivi segment**, le programme crée automatiquement un segment contenant les mêmes contacts que le segment journalisé.

## <a name="see-also"></a>Voir aussi
[Enregistrement d'interactions](marketing-interactions.md)  
[Gestion des contacts](marketing-contacts.md)  
[Gérer les opportunités de ventes](marketing-manage-sales-opportunities.md)  
[Configuration de la gestion du marketing et des contacts](marketing-setup-marketing.md)

