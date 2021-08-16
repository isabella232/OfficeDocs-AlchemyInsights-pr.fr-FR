---
title: Chiffrer automatiquement Office 365 messages électroniques envoyés à certains domaines
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082184"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Chiffrer automatiquement Office 365 messages électroniques envoyés à certains domaines

1. Dans le centre [Exchange' administration,](https://outlook.office365.com/ecp/)choisissez **flux de messagerie > règles.** 
2. Cliquez sur **l’icône Nouveau (+),** puis sur Appliquer chiffrement de messages Office 365 protection des droits **aux messages.**
3. In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.
4. In **Apply this rule if**, choose The recipient > domain **is**. 
5. Entrez le nom du domaine, tel que **contoso.com**.
6. Cliquez sur **l’icône Ajouter (+),** puis sur **OK.**
7. En plus du **champ Faire le champ** Suivant, cliquez sur Sélectionner **un**. 
8. Dans le menu **déroulant du modèle RMS,** sélectionnez **Chiffrer,** puis cliquez sur **OK.** (Si cette option n’est pas disponible, cela signifie que votre plan n’inclut pas le chiffrement automatique. Mais vous pouvez l’ajouter !)
9. Choisissez n’importe quelle sélection facultative (dans une liste de sélections facultatives que vous pouvez effectuer à ce stade, dont la plupart peuvent être laissées avec le paramètre par défaut pour plus de simplicité).
10. Cliquez sur **Save (Enregistrer)**.

> [!IMPORTANT]
> Vous pouvez toujours revenir et modifier cette règle ultérieurement.

Pour plus d’informations sur la création de règles de chiffrement, voir Définir des règles de flux de messagerie pour [chiffrer](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) les messages électroniques dans Office 365