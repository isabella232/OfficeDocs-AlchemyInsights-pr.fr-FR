---
title: Définir des réponses automatiques pour une boîte aux lettres
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046606"
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
