---
title: Écriture écriture/écriture de périphérique
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255155"
---
# <a name="device-writeback"></a><span data-ttu-id="b9c89-102">Écriture écriture/écriture de périphérique</span><span class="sxs-lookup"><span data-stu-id="b9c89-102">Device Writeback</span></span>

<span data-ttu-id="b9c89-103">L’écriture écriture sur appareil est utilisée dans les scénarios suivants :</span><span class="sxs-lookup"><span data-stu-id="b9c89-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="b9c89-104">Activer [Windows Hello Entreprise à l’aide d’un déploiement d’autorisation de certificat hybride](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="b9c89-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="b9c89-105">Activer l’accès conditionnel basé sur les appareils aux applications protégées ADFS (2012 R2 ou supérieure) (approbations de partie de confiance)</span><span class="sxs-lookup"><span data-stu-id="b9c89-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="b9c89-106">Un abonnement à Azure AD Premium est requis pour l’écriture sur l’appareil.</span><span class="sxs-lookup"><span data-stu-id="b9c89-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="b9c89-107">Cela fournit une sécurité et une assurance supplémentaires que l’accès aux applications est accordé uniquement aux appareils de confiance.</span><span class="sxs-lookup"><span data-stu-id="b9c89-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="b9c89-108">Pour plus d’informations sur l’accès conditionnel, voir [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and Setting up [On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span><span class="sxs-lookup"><span data-stu-id="b9c89-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="b9c89-109">Pour plus d’informations sur l’activation de l’écriture écriture sur appareil pour les appareils, voir [Activer l’écriture écriture sur périphérique.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="b9c89-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
