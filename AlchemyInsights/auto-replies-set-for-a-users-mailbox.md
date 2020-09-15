---
title: Définir des réponses automatiques pour une boîte aux lettres
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715127"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Définir des réponses automatiques pour la boîte aux lettres d'un utilisateur

**Méthode 1**

1. Connectez-vous au portail Microsoft 365.

2. Accédez à **Utilisateurs > Utilisateurs actifs** (ou **Groupes > Boîtes aux lettres partagées** si vous les configurez dans une boîte aux lettres partagée).

3. Sélectionnez un utilisateur disposant d’une boîte aux lettres Microsoft Exchange.

4. Dans le menu contextuel sur la droite, accédez à **Paramètres de courrier > Réponses automatiques** (s’il s’agit d’une boîte aux lettres partagée, cliquez simplement sur **Réponses automatiques** à la volée).

**Méthode 2**

1. Connectez-vous au portail d’administration de Microsoft 365 à l’aide des informations d’identification d’administrateur.

2. Développez **Centres d’administration**, puis cliquez sur **Exchange**.

3. Cliquez sur l’image dans le coin supérieur droit, cliquez sur **Autre utilisateur**, puis sélectionnez la boîte aux lettres de l’utilisateur que vous voulez modifier.

4. Sur le côté gauche, sélectionnez **Options**, cliquez sur **Organiser le courrier**, puis sur **Réponses automatiques.**

**Méthode 3**

Dans Exchange Online PowerShell, exécutez l’applet de commande suivantes :

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Pour plus d'informations sur cette applet de commande, voir [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
