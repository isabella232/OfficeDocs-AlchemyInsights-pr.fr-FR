---
title: Corriger les problèmes d’installation de DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744948"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="83614-102">Corriger les problèmes d’installation de DKIM</span><span class="sxs-lookup"><span data-stu-id="83614-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="83614-103">Si vous rencontrez des problèmes d’activation de DKIM pour votre domaine personnalisé, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="83614-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="83614-104">La plupart des problèmes d’installation de DKIM sont liés à des enregistrements DNS incorrects.</span><span class="sxs-lookup"><span data-stu-id="83614-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="83614-105">Vérifiez que l’enregistrement CNAMe DKIM (et**non** un enregistrement txt) est correctement mis en forme.</span><span class="sxs-lookup"><span data-stu-id="83614-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="83614-106">Pour plus d’informations, consultez cette [rubrique](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="83614-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="83614-107">Une fois que vous avez créé ou mis à jour vos enregistrements DNS DKIM au niveau du service d’hébergement DNS pour votre domaine (en général, votre bureau d’enregistrement de domaines), attendez que les enregistrements DNS se propagent.</span><span class="sxs-lookup"><span data-stu-id="83614-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="83614-108">Si vous ne pouvez pas créer les enregistrements DNS DKIM dans le centre d’administration, vous pouvez remplacer \<CustomDomain\> par votre domaine personnalisé (par exemple, contoso.com) et exécuter cette commande dans [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="83614-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
