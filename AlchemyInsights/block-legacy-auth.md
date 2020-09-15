---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685596"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="c5f65-102">Blocage de l’authentification héritée</span><span class="sxs-lookup"><span data-stu-id="c5f65-102">Blocking legacy authentication</span></span>

<span data-ttu-id="c5f65-103">Le terme authentification héritée fait référence à une demande d’authentification effectuée par :</span><span class="sxs-lookup"><span data-stu-id="c5f65-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="c5f65-104">Anciens clients Office qui n’utilisent pas l’authentification moderne (par exemple, le client Office 2010).</span><span class="sxs-lookup"><span data-stu-id="c5f65-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="c5f65-105">Tout client qui utilise des protocoles de messagerie hérités tels que IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="c5f65-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="c5f65-106">Pour plus d’informations sur le blocage de l’authentification héritée et l’activation de l’authentification moderne, consultez la rubrique [blocage de l’authentification héritée](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="c5f65-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="c5f65-107">Les paramètres de sécurité par défaut d’Azure Active Directory (Azure AD) facilitent la sécurisation et la protection de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="c5f65-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="c5f65-108">Les paramètres de sécurité par défaut contiennent des paramètres de sécurité préconfigurés pour les attaques courantes.</span><span class="sxs-lookup"><span data-stu-id="c5f65-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="c5f65-109">Pour plus d’informations sur les paramètres de sécurité par défaut, reportez-vous à la rubrique [Quels sont les paramètres de sécurité par défaut ?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="c5f65-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="c5f65-110">**Remarque**: Si votre client a été créé le 22 octobre, 2019, il est possible que vous rencontriez le nouveau comportement sécurisé par défaut et que les paramètres de sécurité par défaut soient activés dans votre client.</span><span class="sxs-lookup"><span data-stu-id="c5f65-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="c5f65-111">Dans le but de protéger tous nos utilisateurs, les paramètres de sécurité par défaut sont déployés pour tous les nouveaux locataires créés.</span><span class="sxs-lookup"><span data-stu-id="c5f65-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
