---
title: Résoudre les problèmes courants liés à la mise en forme des enregistrement DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500824"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="4c0e7-102">Résoudre les problèmes courants liés à la mise en forme des enregistrement DKIM</span><span class="sxs-lookup"><span data-stu-id="4c0e7-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="4c0e7-103">La plupart des problèmes de mise en place DKIM sont liés à des enregistrements DNS incorrects.</span><span class="sxs-lookup"><span data-stu-id="4c0e7-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="4c0e7-104">Pour résoudre les problèmes de mise en place de DKIM, vérifiez que l’enregistrement CNAME DKIM **(et** non un enregistrement TXT) est correctement mis en forme.</span><span class="sxs-lookup"><span data-stu-id="4c0e7-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="4c0e7-105">Pour plus d’informations, voir ce que vous devez faire pour configurer [manuellement DKIM dans Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)</span><span class="sxs-lookup"><span data-stu-id="4c0e7-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="4c0e7-106">Si vous avez besoin d’aide générale sur les enregistrements DNS, voir Créer des enregistrements DNS auprès d’un fournisseur d’hébergement [DNS pour Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="4c0e7-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="4c0e7-107">Après avoir créé ou mis à jour vos enregistrements DNS DKIM au niveau du service d’hébergement DNS de votre domaine, vous devez attendre que les enregistrements DNS se propagent.</span><span class="sxs-lookup"><span data-stu-id="4c0e7-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
