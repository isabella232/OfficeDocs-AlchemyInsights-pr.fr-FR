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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398558"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="2fd9a-102">Concepts d’authentification avancés applicables à Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2fd9a-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="2fd9a-103">Voici les concepts d’authentification avancés applicables à Microsoft Edge :</span><span class="sxs-lookup"><span data-stu-id="2fd9a-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="2fd9a-104">**Authentification proactive**</span><span class="sxs-lookup"><span data-stu-id="2fd9a-104">**Proactive Authentication**</span></span>

<span data-ttu-id="2fd9a-105">Lorsque vous activez la stratégie [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge tente d’authentifier de manière proactive les utilisateurs inscrits via les services Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2fd9a-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="2fd9a-106">À intervalles réguliers, il utilise un service en ligne pour vérifier un manifeste mis à jour qui contient la configuration régissant l’authentification proactive.</span><span class="sxs-lookup"><span data-stu-id="2fd9a-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="2fd9a-107">Avantages : l’authentification proactive permet l’authentification à des services clés, tels que la page Nouvel onglet Office.</span><span class="sxs-lookup"><span data-stu-id="2fd9a-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="2fd9a-108">En outre, si Bing est utilisé comme moteur de recherche, l’authentification proactive améliore les performances de la barre d’adresses et permet de générer des résultats de recherche personnalisés en fonction des besoins de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="2fd9a-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="2fd9a-109">**Windows Hello CredUI pour l’authentification NTLM**</span><span class="sxs-lookup"><span data-stu-id="2fd9a-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="2fd9a-110">Si l’authentification unique (SSO) n’est pas disponible lorsqu’un site web tente de se connecter à l’utilisateur via le mécanisme NTLM ou Negotiate, cette fonctionnalité permet à l’utilisateur de partager les informations d’identification du système d’exploitation avec le site web et de répondre au défi d’authentification à l’aide de Windows Hello Cred UI.</span><span class="sxs-lookup"><span data-stu-id="2fd9a-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="2fd9a-111">Ce flux d' sign-on s’affiche uniquement dans Windows 10 et uniquement pour les utilisateurs qui n’obtiennent pas d' SSO pendant une demande NTLM ou Negotiate.</span><span class="sxs-lookup"><span data-stu-id="2fd9a-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="2fd9a-112">**Utiliser des mots de passe enregistrés pour se connecter automatiquement**</span><span class="sxs-lookup"><span data-stu-id="2fd9a-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="2fd9a-113">Les utilisateurs qui enregistrent des mots de passe dans Microsoft Edge peuvent activer la connexion automatique aux sites web où ils ont enregistré des informations d’identification.</span><span class="sxs-lookup"><span data-stu-id="2fd9a-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="2fd9a-114">Les utilisateurs peuvent activer ou désactiver cette fonctionnalité dans edge://settings/passwords, et vous pouvez la configurer dans les stratégies du [gestionnaire de mots de](https://go.microsoft.com/fwlink/?linkid=2134622) passe.</span><span class="sxs-lookup"><span data-stu-id="2fd9a-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
