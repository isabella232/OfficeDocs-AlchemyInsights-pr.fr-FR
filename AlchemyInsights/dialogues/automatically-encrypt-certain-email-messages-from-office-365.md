---
title: Chiffrer automatiquement certains messages électroniques à partir d’Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509915"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Chiffrer automatiquement certains messages électroniques à partir d’Office 365

1. Dans le Centre [d’administration Exchange,](https://outlook.office365.com/ecp/)sélectionnez **flux de messagerie > règles.** 
2. Cliquez sur **l’icône Nouveau (+),** puis cliquez sur Appliquer le chiffrement de messages **Office 365** et la protection des droits aux messages.
3. In **Name**, enter a name for the rule, such as *Encrypt all messages*.
4. In **Apply this rule if**, choose **[Apply to all messages]**. 
5. En plus du **champ Faire le champ** Suivant, cliquez sur Sélectionner **un**. 
6. Dans le menu **déroulant du modèle RMS,** sélectionnez **Chiffrer,** puis cliquez sur **OK.** (Si cette option n’est pas disponible, cela signifie que votre plan n’inclut pas le chiffrement automatique. Mais vous pouvez l’ajouter !)
7. Cochez **la case Auditer** cette règle avec le niveau de gravité, puis sélectionnez le niveau souhaité. Si votre entreprise a des obligations contractuelles d’envoyer tous les e-mails chiffrés, je vous recommande de définir le niveau sur **Élevé**.
8. Sous **Choisir un modèle pour cette règle,** cliquez sur **Appliquer.** 
9. Choisissez n’importe quelle sélection facultative (dans une liste de sélections facultatives que vous pouvez effectuer à ce stade, dont la plupart peuvent être laissées avec le paramètre par défaut par souci de simplicité).
10. Cliquez sur **Enregistrer**.

> [!IMPORTANT]
> Vous pouvez toujours revenir et modifier cette règle ultérieurement.

Pour plus d’informations sur la création de règles de chiffrement, voir Définir des règles de flux de messagerie pour chiffrer les [messages électroniques dans Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

