---
title: Définir des réponses automatiques pour la boîte aux lettres d'un utilisateur
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506458"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Définir des réponses automatiques pour la boîte aux lettres d'un utilisateur

**Méthode 1**

1. Se connecter au portail Office 365.

2. Accédez à **Utilisateurs > Utilisateurs actifs** (ou **Groupes > Boîtes aux lettres partagées** si vous les configurez dans une boîte aux lettres partagée).

3. Sélectionnez un utilisateur disposant d’une boîte aux lettres Microsoft Exchange.

4. Dans le menu contextuel sur la droite, accédez à **Paramètres de courrier > Réponses automatiques** (s’il s’agit d’une boîte aux lettres partagée, cliquez simplement sur **Réponses automatiques** à la volée).

**Méthode 2**

1. Connectez-vous au Portail d’administration Office 365 à l’aide des informations d’identification d’administrateur.

2. Développez **Centres d’administration**, puis cliquez sur **Exchange**.

3. Cliquez sur l’image dans le coin supérieur droit, cliquez sur **Autre utilisateur**, puis sélectionnez la boîte aux lettres de l’utilisateur que vous voulez modifier.

4. Sur le côté gauche, sélectionnez **Options**, cliquez sur **Organiser le courrier**, puis sur **Réponses automatiques.**

**Méthode 3**

Dans Exchange Online PowerShell, exécutez l’applet de commande suivantes :

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

Pour plus d'informations sur cette applet de commande, voir [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
