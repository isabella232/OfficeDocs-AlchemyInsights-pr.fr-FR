---
title: L’accès conditionnel avec un appareil joint au domaine me bloque
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965463"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="bf5b4-102">L’accès conditionnel avec un appareil joint au domaine me bloque</span><span class="sxs-lookup"><span data-stu-id="bf5b4-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="bf5b4-103">**Outils hautement recommandés**</span><span class="sxs-lookup"><span data-stu-id="bf5b4-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="bf5b4-104">[Outil de résolution des problèmes d’alignement des appareils](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) : outil qui vous aide à résoudre les problèmes les plus courants d’alignement des appareils.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="bf5b4-105">[Script de connectivité pour l'alignement des appareils de test](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : script contribuant à garantir qu’un appareil peut accéder aux points de terminaison d’alignement des appareils sous le compte système.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="bf5b4-106">[Script de nettoyage d’appareil Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) : script qui vous permet de rechercher, puis de gérer les appareils obsolètes dans votre environnement.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="bf5b4-107">Voici quelques-unes des raisons courantes pour lesquelles l’accès conditionnel peut échouer sur un appareil qui a rejoint un domaine (Azure AD Hybride).</span><span class="sxs-lookup"><span data-stu-id="bf5b4-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="bf5b4-108">**Aucun jeton d’actualisation principal Azure AD n’existe sur l’appareil** : vous devez vérifier que l’appareil contient le jeton d’actualisation principal Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="bf5b4-109">Si vous souhaitez en savoir plus le jeton d’actualisation principal, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="bf5b4-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="bf5b4-110">Pour vérifier si vous avez le jeton d’actualisation principal Azure AD, vous pouvez exécuter la commande `dsregcmd/status` sur l’appareil, puis vérifier si « AzureAdPrt » a la valeur « YES ».</span><span class="sxs-lookup"><span data-stu-id="bf5b4-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="bf5b4-111">Si « AzureAdPrt » a la valeur « NO », vérifiez les points suivants :</span><span class="sxs-lookup"><span data-stu-id="bf5b4-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="bf5b4-112">**Si vous avez un environnement fédéré avec AD FS et qu’il est inaccessible aux réseaux d’accueil de vos utilisateurs** : dans ce cas, vérifiez que vos points de terminaison « usernamemixed » sont accessibles depuis l’extranet.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="bf5b4-113">Si votre service AD FS se trouve derrière un VPN, vérifiez que les utilisateurs se connectent au VPN, puis se connectent de nouveau à l’appareil.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="bf5b4-114">Si vous souhaitez en savoir plus, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="bf5b4-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="bf5b4-115">**Déterminer si le module de plateforme sécurisée de l’appareil est défectueux et ne peut donc pas authentifier l’appareil** : vérifiez « tpm.msc » pour déterminer si l’état du l’appareil est « Prêt ».</span><span class="sxs-lookup"><span data-stu-id="bf5b4-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="bf5b4-116">Si ce n’est pas le cas, exécutez `dsregcmd/leave`, puis laissez l’appareil se joindre de nouveau à Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="bf5b4-117">Réessayez ensuite.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-117">Then, try again.</span></span> <span data-ttu-id="bf5b4-118">Si vous souhaitez en savoir plus, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="bf5b4-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="bf5b4-119">**Vous utilisez un fournisseur d’identité tiers, qui ne prend pas en charge les protocoles WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="bf5b4-120">Comme décrit dans nos documents, les appareils joints à Azure AD Hybride ne peuvent pas fonctionner dans ce cas.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="bf5b4-121">Veuillez contacter votre fournisseur d’identité pour obtenir du support.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="bf5b4-122">**Les utilisateurs utilisent le navigateur Chrome sans les comptes Windows 10** ou **l’extension Office Chrome n’utilise pas automatiquement le jeton d’actualisation principal sur des appareils joints à AAD ou AAD Hybride** : cela entraîne l’échec de toutes les stratégies d’accès conditionnel basées sur les appareils, avec le message d’erreur « Appareil non inscrit » affiché.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="bf5b4-123">Pour utiliser correctement le navigateur Chrome, vous devez installer les « comptes Windows 10 » ou « l'extension d’Office au navigateur Chrome des utilisateurs » via SCCM ou Intune.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="bf5b4-124">Si vous souhaitez en savoir plus, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="bf5b4-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="bf5b4-125">S’il n’est pas possible d’envoyer (push) l’extension à distance, dites aux utilisateurs d’installer manuellement d’une des extensions ci-dessus pour accéder aux applications derrière l’accès conditionnel basé sur l’appareil.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="bf5b4-126">Si vous souhaitez en savoir plus, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="bf5b4-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="bf5b4-127">**Vous avez correctement joint l’appareil à Azure AD Hybride, mais vous l’avez supprimé ou désactivé par inadvertance, en raison de modifications de synchronisation dans Azure AD Connect ou depuis le portail Azure** : dans ce cas, le programme ne reconnaît plus l’objet de l’appareil comme un appareil complètement joint, même si les statuts « AzureAdJoined » et « PRT » apparaissent comme valides sur l’appareil.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="bf5b4-128">Pour résoudre ce problème, exécutez la commande `dsregcmd/leave` sur les appareils concernés, puis laissez-les rejoindre Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="bf5b4-129">Si vous souhaitez en savoir plus, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="bf5b4-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="bf5b4-130">Si vos appareils sont sous Windows 10, mise à jour 1809, avec un proxy VPN/cloud et que vous voyez des problèmes d’état « AzureAdPrt » ou toute application avec un problème d'authentification unique (Outlook ne se connecte pas à la boîte aux lettres même si vous aviez un jeton d’actualisation principal), vérifiez que vous avez ce correctif [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ou la mise à jour cumulative d’avril [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) pour éviter les défaillances du jeton d’actualisation principal sur ces ordinateurs.</span><span class="sxs-lookup"><span data-stu-id="bf5b4-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















