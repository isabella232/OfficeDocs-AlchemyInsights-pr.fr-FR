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
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="1a396-102">Définir des réponses automatiques pour la boîte aux lettres d'un utilisateur</span><span class="sxs-lookup"><span data-stu-id="1a396-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="1a396-103">**Méthode 1**</span><span class="sxs-lookup"><span data-stu-id="1a396-103">**Method 1**</span></span>

1. <span data-ttu-id="1a396-104">Se connecter au portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="1a396-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="1a396-105">Accédez à **Utilisateurs > Utilisateurs actifs** (ou **Groupes > Boîtes aux lettres partagées** si vous les configurez dans une boîte aux lettres partagée).</span><span class="sxs-lookup"><span data-stu-id="1a396-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="1a396-106">Sélectionnez un utilisateur disposant d’une boîte aux lettres Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a396-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="1a396-107">Dans le menu contextuel sur la droite, accédez à **Paramètres de courrier > Réponses automatiques** (s’il s’agit d’une boîte aux lettres partagée, cliquez simplement sur **Réponses automatiques** à la volée).</span><span class="sxs-lookup"><span data-stu-id="1a396-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="1a396-108">**Méthode 2**</span><span class="sxs-lookup"><span data-stu-id="1a396-108">**Method 2**</span></span>

1. <span data-ttu-id="1a396-109">Connectez-vous au Portail d’administration Office 365 à l’aide des informations d’identification d’administrateur.</span><span class="sxs-lookup"><span data-stu-id="1a396-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="1a396-110">Développez **Centres d’administration**, puis cliquez sur **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="1a396-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="1a396-111">Cliquez sur l’image dans le coin supérieur droit, cliquez sur **Autre utilisateur**, puis sélectionnez la boîte aux lettres de l’utilisateur que vous voulez modifier.</span><span class="sxs-lookup"><span data-stu-id="1a396-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="1a396-112">Sur le côté gauche, sélectionnez **Options**, cliquez sur **Organiser le courrier**, puis sur **Réponses automatiques.**</span><span class="sxs-lookup"><span data-stu-id="1a396-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="1a396-113">**Méthode 3**</span><span class="sxs-lookup"><span data-stu-id="1a396-113">**Method 3**</span></span>

<span data-ttu-id="1a396-114">Dans Exchange Online PowerShell, exécutez l’applet de commande suivantes :</span><span class="sxs-lookup"><span data-stu-id="1a396-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="1a396-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="1a396-115">PowerShellCopy</span></span>

    Set-MailboxAutoReplyConfiguration

<span data-ttu-id="1a396-116">Pour plus d'informations sur cette applet de commande, voir [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="1a396-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
