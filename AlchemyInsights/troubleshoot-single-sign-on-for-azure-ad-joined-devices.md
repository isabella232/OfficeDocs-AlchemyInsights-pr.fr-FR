---
title: Résoudre les problèmes d' sign-on unique pour les appareils joints à Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897741"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="5158a-102">Résoudre les problèmes d' sign-on unique pour les appareils joints à Azure AD</span><span class="sxs-lookup"><span data-stu-id="5158a-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="5158a-103">Si vous avez un environnement Active Directory (AD) local et que vous souhaitez joindre vos ordinateurs joints à un domaine AD à Azure AD, vous pouvez le faire en rejoignant Azure AD hybride.</span><span class="sxs-lookup"><span data-stu-id="5158a-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="5158a-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="5158a-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="5158a-105">Pour plus d’informations, voir Configurer les appareils joints à Azure AD pour l'Single-Sign sur site à l’aide [de Windows Hello Entreprise.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="5158a-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="5158a-106">**Problèmes de jeton d’actualisation principal (PRT)**</span><span class="sxs-lookup"><span data-stu-id="5158a-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="5158a-107">Un jeton d’actualisation principal (PRT) est un artefact clé de l’authentification Azure AD sur les appareils Windows 10, Windows Server 2016 et versions ultérieures, iOS et Android.</span><span class="sxs-lookup"><span data-stu-id="5158a-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="5158a-108">Il s’agit d’un jeton web JSON (JWT) spécialement envoyé aux courtiers de jetons microsoft pour activer l' sign-on unique (SSO) sur les applications utilisées sur ces appareils.</span><span class="sxs-lookup"><span data-stu-id="5158a-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="5158a-109">Pour plus d’informations sur la façon dont un PRT est émis, utilisé et protégé sur les appareils Windows 10, voir Qu’est-ce qu’un jeton [d’actualisation principal ?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="5158a-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="5158a-110">**WamDefaultSet : OUI et AzureADPrt : OUI**</span><span class="sxs-lookup"><span data-stu-id="5158a-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="5158a-111">Ces champs indiquent si l’utilisateur s’est authentifié avec succès à Azure AD lors de la signature de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="5158a-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="5158a-112">Si les valeurs sont **NO,** cela peut être dû à :</span><span class="sxs-lookup"><span data-stu-id="5158a-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="5158a-113">Clé de stockage non bonne dans le TPM associé à l’appareil lors de l’inscription (vérifiez keySignTest lors de l’exécution avec élévation de niveau)</span><span class="sxs-lookup"><span data-stu-id="5158a-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="5158a-114">Autre ID de connexion</span><span class="sxs-lookup"><span data-stu-id="5158a-114">Alternate Login ID</span></span>
- <span data-ttu-id="5158a-115">Proxy HTTP in trouvé</span><span class="sxs-lookup"><span data-stu-id="5158a-115">HTTP Proxy not found</span></span>

<span data-ttu-id="5158a-116">Pour résoudre les problèmes d’appareils à l’aide de la commande dsregcmd, consultez [l’état de l' cesso.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="5158a-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
