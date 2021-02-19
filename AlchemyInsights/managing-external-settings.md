---
title: Gestion des paramètres externes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282815"
---
# <a name="managing-external-settings"></a><span data-ttu-id="23733-102">Gestion des paramètres externes</span><span class="sxs-lookup"><span data-stu-id="23733-102">Managing External Settings</span></span>

<span data-ttu-id="23733-103">**Annonce**</span><span class="sxs-lookup"><span data-stu-id="23733-103">**Announcement**</span></span>

- <span data-ttu-id="23733-104">[Prise en charge de la connexion à WebView depuis Google déconseillée à compter du 4 janvier 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="23733-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="23733-105">Vérifiez si cela concerne vos applications en suivant les conseils de Google sur les tests de compatibilité</span><span class="sxs-lookup"><span data-stu-id="23733-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="23733-106">Veillez à utiliser le système webview ou le navigateur système lorsque vous connectez à vos utilisateurs avec des comptes Google grand public</span><span class="sxs-lookup"><span data-stu-id="23733-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="23733-107">**Gérer les paramètres d’invitation**</span><span class="sxs-lookup"><span data-stu-id="23733-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="23733-108">Confirmez que vous avez [configuré les paramètres de collaboration externe](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) pour autoriser les personnes appropriées à envoyer des invitations.</span><span class="sxs-lookup"><span data-stu-id="23733-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="23733-109">**Gérer les autorisations d’accès des utilisateurs invités**</span><span class="sxs-lookup"><span data-stu-id="23733-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="23733-110">Les administrateurs globaux peuvent gérer les autorisations d’accès invité dans l’annuaire via le portail Azure en configurant les autorisations d’accès invité dans la page External Collaboration Settings (Paramètres de collaboration externe).</span><span class="sxs-lookup"><span data-stu-id="23733-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="23733-111">[En savoir plus sur ce paramètre](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="23733-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="23733-112">Si vous voulez que vos invités accèdent à des applications telles que Teams ou SharePoint, confirmez que vous les avez configurées pour autoriser l’accès invité.</span><span class="sxs-lookup"><span data-stu-id="23733-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="23733-113">En savoir plus sur les paramètres [Teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) et [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="23733-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="23733-114">**Configuration d’invitations :**</span><span class="sxs-lookup"><span data-stu-id="23733-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="23733-115">Activer la collaboration externe B2B, puis gérer les utilisateurs pouvant avoir des invités</span><span class="sxs-lookup"><span data-stu-id="23733-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- <span data-ttu-id="23733-116">[Autoriser ou bloquer des invitations à des utilisateurs depuis des organisations spécifiques](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="23733-116">[Allow or block invitations to users from specific organizations](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="23733-117">**Configuration des fournisseurs d’identité autorisés :**</span><span class="sxs-lookup"><span data-stu-id="23733-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="23733-118">Fédération Google</span><span class="sxs-lookup"><span data-stu-id="23733-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="23733-119">Fédération directe</span><span class="sxs-lookup"><span data-stu-id="23733-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="23733-120">Authentification par envoi d’un code secret unique par e-mail</span><span class="sxs-lookup"><span data-stu-id="23733-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
