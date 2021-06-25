---
title: Activer l'authentification et le dépannage SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077649"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="3b7e7-102">Activer l'authentification et le dépannage SMTP</span><span class="sxs-lookup"><span data-stu-id="3b7e7-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="3b7e7-103">Si vous souhaitez activer l’authentification SMTP pour une boîte aux lettres ou si vous obtenez une erreur « Client non authentifié », « Échec de l’authentification » ou « SmtpClientAuthentication » avec le code 5.7.57 ou 5.7.3 ou 5.7.139 lorsque vous tentez de relayer le courrier en authentifiant un appareil ou une application avec Microsoft 365, effectuez ces trois actions pour résoudre le problème :</span><span class="sxs-lookup"><span data-stu-id="3b7e7-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="3b7e7-104">Désactivez [les valeurs par défaut de la sécurité d 'Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)en mettant l'option **Activer les valeurs par défaut** de la sécurité sur **Non**.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="3b7e7-105">a.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-105">a.</span></span> <span data-ttu-id="3b7e7-106">Connectez-vous au portail Azure en tant qu'administrateur de sécurité, administrateur d'accès conditionnel ou administrateur global.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="3b7e7-107">b.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-107">b.</span></span> <span data-ttu-id="3b7e7-108">Naviguez jusqu'à Azure Active Directory >  **Propriétés**.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="3b7e7-109">c.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-109">c.</span></span> <span data-ttu-id="3b7e7-110">Sélectionnez **Gérer les paramètres de sécurité par défaut**.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="3b7e7-111">d.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-111">d.</span></span> <span data-ttu-id="3b7e7-112">Définir **l'activation de la sécurité par défaut** sur **Non**.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="3b7e7-113">e.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-113">e.</span></span> <span data-ttu-id="3b7e7-114">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-114">Select **Save**.</span></span>

2. <span data-ttu-id="3b7e7-115">[Activez la soumission SMTP du client](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) sur la boîte aux lettres sous licence.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="3b7e7-116">a.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-116">a.</span></span> <span data-ttu-id="3b7e7-117">Dans le centre d'administration de Microsoft 365, accédez à **Utilisateurs actifs** , puis sélectionnez l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="3b7e7-118">b.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-118">b.</span></span> <span data-ttu-id="3b7e7-119">Allez dans l'onglet Courrier, et sous **Applications de messagerie**, sélectionnez **Gérer les applications** de messagerie.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="3b7e7-120">d.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-120">d.</span></span> <span data-ttu-id="3b7e7-121">Assurez-vous que la case **Authenticated SMTP** est cochée (activée).</span><span class="sxs-lookup"><span data-stu-id="3b7e7-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="3b7e7-122">e.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-122">e.</span></span> <span data-ttu-id="3b7e7-123">Sélectionnez **Enregistrer les modifications**.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="3b7e7-124">[Désactiver l'authentification multifactorielle (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) sur la boîte aux lettres sous licence.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="3b7e7-125">a.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-125">a.</span></span> <span data-ttu-id="3b7e7-126">Allez dans le centre d'administration de Microsoft 365, et dans le menu de navigation de gauche, sélectionnez **Utilisateurs** > **Utilisateurs actifs**.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="3b7e7-127">b.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-127">b.</span></span> <span data-ttu-id="3b7e7-128">Sélectionnez **Authentification multifactorielle**.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="3b7e7-129">c.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-129">c.</span></span> <span data-ttu-id="3b7e7-130">Sélectionnez l'utilisateur et désactivez **l'authentification multifactorielle**.</span><span class="sxs-lookup"><span data-stu-id="3b7e7-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
