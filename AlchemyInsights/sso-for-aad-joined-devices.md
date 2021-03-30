---
title: Single-Sign active pour les appareils joints à Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403796"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="3d0fc-102">Sign-on unique pour les appareils joints à Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="3d0fc-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="3d0fc-103">Si vous avez un environnement Active Directory (AD) local et que vous souhaitez joindre vos ordinateurs joints à un domaine AD à Azure AD, vous pouvez le faire en rejoignant Azure AD hybride.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="3d0fc-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="3d0fc-105">Configurer des appareils joints à Azure AD pour l'Single-Sign sur site à l’aide de Windows Hello Entreprise</span><span class="sxs-lookup"><span data-stu-id="3d0fc-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="3d0fc-106">**Problèmes de jeton d’actualisation principal (PRT)** Un jeton d’actualisation principal (PRT) est un artefact clé de l’authentification Azure AD sur les appareils Windows 10, Windows Server 2016 et versions ultérieures, iOS et Android.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="3d0fc-107">Il s’agit d’un jeton web JSON (JWT) spécialement envoyé aux courtiers de jetons microsoft pour activer l' sign-on unique (SSO) sur les applications utilisées sur ces appareils.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="3d0fc-108">[Dans Qu’est-ce qu’un](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)jeton d’actualisation principal ? , nous fournirons des détails sur la façon dont un prt est émis, utilisé et protégé sur les appareils Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="3d0fc-109">**WamDefaultSet : OUI et AzureADPrt : OUI** Ces champs indiquent si l’utilisateur s’est authentifié avec succès à Azure AD lors de la signature de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="3d0fc-110">Si les valeurs sont **NO,** cela peut être dû :</span><span class="sxs-lookup"><span data-stu-id="3d0fc-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="3d0fc-111">Clé de stockage non bonne dans le TPM associé à l’appareil lors de l’inscription (vérifiez keySignTest lors de l’exécution avec élévation de niveau).</span><span class="sxs-lookup"><span data-stu-id="3d0fc-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="3d0fc-112">Autre ID de connexion</span><span class="sxs-lookup"><span data-stu-id="3d0fc-112">Alternate Login ID</span></span>
- <span data-ttu-id="3d0fc-113">Proxy HTTP in trouvé</span><span class="sxs-lookup"><span data-stu-id="3d0fc-113">HTTP Proxy not found</span></span>

<span data-ttu-id="3d0fc-114">Résoudre les problèmes d’appareils à l’aide de la commande dsregcmd - [État de l' sso](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="3d0fc-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
