---
title: Chiffrer automatiquement certains messages Office 365 courrier électronique
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: b15a72ced4921b3df1b7105837592781188a2a25
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327972"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Chiffrer automatiquement certains messages Office 365 courrier électronique

Vous pouvez chiffrer automatiquement les messages que les utilisateurs envoient à certaines personnes ou organisations externes. Pour ce faire, procédez comme suit :

1. Dans le centre [Exchange' administration,](https://outlook.office365.com/ecp/)choisissez **flux de messagerie > règles.** 
2. Cliquez sur **l’icône Nouveau (+),** puis sur Appliquer chiffrement de messages Office 365 protection des droits **aux messages.**
3. In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.
4. In **Apply this rule if**, choose The recipient > is this **person**. 
5. Dans la **fenêtre Sélectionner des** membres, sélectionnez le nom de la personne à qui la règle de chiffrement doit s’appliquer, puis cliquez sur **Ajouter.** 
6. Lorsque vous avez terminé d’ajouter des utilisateurs, cliquez **sur OK.**
7. En plus du **champ Faire le champ** Suivant, cliquez sur Sélectionner **un**. 
8. Dans le menu **déroulant du modèle RMS,** sélectionnez **Chiffrer,** puis cliquez sur **OK.** (Si cette option n’est pas disponible, cela signifie que votre plan n’inclut pas le chiffrement automatique. Mais vous pouvez l’ajouter !)
9. Choisissez n’importe quelle sélection facultative (dans une liste de sélections facultatives que vous pouvez effectuer à ce stade, dont la plupart peuvent être laissées avec le paramètre par défaut par souci de simplicité).
10. Cliquez sur **Enregistrer**.

**Important**: vous pouvez toujours revenir et modifier cette règle ultérieurement.

Pour plus d’informations sur la création de règles de chiffrement, voir Définir des règles de flux de messagerie pour [chiffrer](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)les messages électroniques Office 365 .

