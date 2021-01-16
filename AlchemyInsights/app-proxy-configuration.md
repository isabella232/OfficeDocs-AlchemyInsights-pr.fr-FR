---
title: Configuration du proxy d’application
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876543"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="bb8cb-102">Configuration du proxy d’application</span><span class="sxs-lookup"><span data-stu-id="bb8cb-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="bb8cb-103">Pour comprendre comment configurer une application proxy d’application dans Azure AD pour exposer vos applications sur site au cloud, voir Comment configurer une [application proxy d’application.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)</span><span class="sxs-lookup"><span data-stu-id="bb8cb-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="bb8cb-104">L’authentification unique (SSO) permet à vos utilisateurs d’accéder à une application sans s’authentifier plusieurs fois.</span><span class="sxs-lookup"><span data-stu-id="bb8cb-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="bb8cb-105">Il permet à l’authentification unique de se produire dans le cloud, par rapport à Azure Active Directory, et permet au service ou au connecteur d’usurper l’identité de l’utilisateur pour relever les défis d’authentification supplémentaires de l’application.</span><span class="sxs-lookup"><span data-stu-id="bb8cb-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="bb8cb-106">Pour plus d’informations, [voir Comment configurer l' sign-on unique sur une application proxy d’application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="bb8cb-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="bb8cb-107">Utilisez [cet article pour](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) résoudre les problèmes courants que rencontrent les personnes lors de la création d’une application proxy d’application.</span><span class="sxs-lookup"><span data-stu-id="bb8cb-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="bb8cb-108">Si vous avez un problème lors de la configuration de l’authentification back-end sur votre application, vous devrez peut-être résoudre les configurations de délégation [Kerberos contraintes](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) pour le proxy d’application ou suivre des instructions sur la configuration de l’application avec [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) pour résoudre votre problème.</span><span class="sxs-lookup"><span data-stu-id="bb8cb-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
