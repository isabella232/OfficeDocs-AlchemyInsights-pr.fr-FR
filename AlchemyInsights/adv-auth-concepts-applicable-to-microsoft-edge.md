---
title: Concepts d’authentification avancés applicables à Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571826"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="0f2d0-102">Concepts d’authentification avancés applicables à Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="0f2d0-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="0f2d0-103">Voici les concepts d’authentification avancés qui s’appliquent à Microsoft Edge :</span><span class="sxs-lookup"><span data-stu-id="0f2d0-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="0f2d0-104">**Authentification proactive**</span><span class="sxs-lookup"><span data-stu-id="0f2d0-104">**Proactive Authentication**</span></span>

<span data-ttu-id="0f2d0-105">Lorsque vous activez la stratégie [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge essaie d’authentifier de manière proactive les utilisateurs connectés via les services Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0f2d0-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="0f2d0-106">À intervalles réguliers, il utilise un service en ligne pour rechercher un manifeste mis à jour qui contient la configuration régissant l’authentification proactive.</span><span class="sxs-lookup"><span data-stu-id="0f2d0-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="0f2d0-107">Avantages : l’authentification proactive permet l’authentification à des services clés, tels que la page Office New Tab.</span><span class="sxs-lookup"><span data-stu-id="0f2d0-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="0f2d0-108">De plus, si Bing est utilisé comme moteur de recherche, l’authentification proactive améliore les performances de la barre d’adresses et génère des résultats de recherche personnalisés pour répondre aux besoins de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="0f2d0-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="0f2d0-109">**Windows Hello CredUI pour l’authentification NTLM**</span><span class="sxs-lookup"><span data-stu-id="0f2d0-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="0f2d0-110">Si l’authentification unique (SSO) n’est pas disponible lorsqu’un site Web tente de se connecter à l’utilisateur par le biais du mécanisme NTLM ou Negotiate, cette fonctionnalité permet à l’utilisateur de partager les informations d’identification du système d’exploitation avec le site Web et de satisfaire la stimulation d’authentification à l’aide de l’interface utilisateur Windows Hello CRED.</span><span class="sxs-lookup"><span data-stu-id="0f2d0-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="0f2d0-111">Ce flux d’authentification s’affiche uniquement dans Windows 10 et uniquement pour les utilisateurs qui n’obtiennent pas d’authentification unique pendant une stimulation NTLM ou Negotiate.</span><span class="sxs-lookup"><span data-stu-id="0f2d0-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="0f2d0-112">**Utiliser des mots de passe enregistrés pour se connecter automatiquement**</span><span class="sxs-lookup"><span data-stu-id="0f2d0-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="0f2d0-113">Les utilisateurs qui enregistrent des mots de passe dans Microsoft Edge peuvent activer la connexion automatique aux sites Web où ils ont enregistré des informations d’identification.</span><span class="sxs-lookup"><span data-stu-id="0f2d0-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="0f2d0-114">Les utilisateurs peuvent activer ou désactiver cette fonctionnalité dans edge://settings/passwords, et vous pouvez les configurer dans les stratégies du [Gestionnaire de mots de passe](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="0f2d0-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
