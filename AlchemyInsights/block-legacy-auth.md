---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820176"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="67489-102">Blocage de l'authentification héritée</span><span class="sxs-lookup"><span data-stu-id="67489-102">Blocking legacy authentication</span></span>

<span data-ttu-id="67489-103">Le terme authentification héritée fait référence à une demande d’authentification effectuée par :</span><span class="sxs-lookup"><span data-stu-id="67489-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="67489-104">Clients Office plus anciens qui n'utilisent pas l'authentification moderne (par exemple, client Office 2010).</span><span class="sxs-lookup"><span data-stu-id="67489-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="67489-105">Tout client qui utilise des protocoles de messagerie hérités tels que IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="67489-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="67489-106">Pour plus d'informations sur le blocage de l'authentification héritée et l'activation de l'authentification moderne, voir [Blocage de l'authentification héritée.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="67489-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="67489-107">Les paramètres de sécurité par défaut dans Azure Active Directory (Azure AD) facilitent la sécurisation et contribuent à protéger votre organisation.</span><span class="sxs-lookup"><span data-stu-id="67489-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="67489-108">Les paramètres de sécurité par défaut contiennent des paramètres de sécurité préconfigurés pour les attaques courantes.</span><span class="sxs-lookup"><span data-stu-id="67489-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="67489-109">Pour plus d'informations sur les paramètres de sécurité par défaut, reportez-vous à [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="67489-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="67489-110">**Remarque**: si votre client a été créé le 22 octobre 2019 ou après celui-ci, il est possible que vous traversiez le nouveau comportement de sécurité par défaut et que les paramètres de sécurité par défaut soient déjà activés dans votre client.</span><span class="sxs-lookup"><span data-stu-id="67489-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="67489-111">Afin de protéger tous nos utilisateurs, les paramètres de sécurité par défaut sont déployés sur tous les nouveaux clients créés.</span><span class="sxs-lookup"><span data-stu-id="67489-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
