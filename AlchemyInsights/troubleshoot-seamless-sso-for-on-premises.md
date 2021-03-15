---
title: Résoudre des problèmes d’authentification unique (SSO) de manière transparente pour l’expérience en local
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753419"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="cb3a6-102">Résoudre des problèmes d’authentification unique (SSO) de manière transparente pour l’expérience en local</span><span class="sxs-lookup"><span data-stu-id="cb3a6-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="cb3a6-103">Pour résoudre les problèmes d'authentification unique (SSO), procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="cb3a6-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="cb3a6-104">**Comment puis-je utiliser la clé de déchiffrement Kerberos du compte d’ordinateur AZUREADSSO ?**</span><span class="sxs-lookup"><span data-stu-id="cb3a6-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="cb3a6-105">Nous vous recommandons vivement de renouveler la clé de déchiffrement Kerberos au moins tous les 30 jours.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="cb3a6-106">Pour ce faire manuellement, consultez [Comment renouveler les clés de déchiffrement Kerberos ?](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="cb3a6-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="cb3a6-107">**Configurer l’authentification unique transparente**</span><span class="sxs-lookup"><span data-stu-id="cb3a6-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="cb3a6-108">Pour déployer l' authentification unique transparente, suivez les étapes [Authentification unique transparente d’Azure Active Directory : démarrage rapide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="cb3a6-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="cb3a6-109">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="cb3a6-109">**Advisory**</span></span>

- <span data-ttu-id="cb3a6-110">[Authentification unique transparente d’Azure Active Directory : questions fréquentes](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) : dans cet article, nous répondons aux questions fréquemment posées sur l'authentification unique transparente d'Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="cb3a6-111">Consultez régulièrement la publication de nouveau contenu.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="cb3a6-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) : cet article fournit des informations sur la façon de poser des demandes de fonctionnalité ou poser des questions techniques sur l'authentification unique transparente.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="cb3a6-113">**Résoudre les problèmes**</span><span class="sxs-lookup"><span data-stu-id="cb3a6-113">**Troubleshoot**</span></span>

<span data-ttu-id="cb3a6-114">[Résoudre des problèmes liés à l’authentification unique transparente d’Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) : cet article vous aide à trouver des informations de dépannage sur les problèmes courants concernant l’authentification unique transparente d’Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="cb3a6-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







