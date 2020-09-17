---
title: Impossible de se connecter à Teams en raison d’une erreur autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799958"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="d7f5a-102">Impossible de se connecter à Teams en raison d’une erreur autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="d7f5a-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="d7f5a-103">Si l’authentification unique transparente est activée comme authentification Office 365, l’URL « autologon.microsoftazuread-sso.com » doit peut-être être ajoutée aux sites intranet.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="d7f5a-104">Si elle a été précédemment ajoutée aux sites de confiance et que l’authentification unique transparente est utilisée, elle doit être supprimée des sites de confiance.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="d7f5a-105">Consultez [la liste de contrôle pour la résolution des problèmes d’authentification unique transparente](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="d7f5a-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="d7f5a-106">Pour ajouter une URL à la liste des sites intranet, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="d7f5a-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="d7f5a-107">Pour ouvrir Internet Explorer, cliquez sur le bouton **démarrer**.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="d7f5a-108">Dans la zone de recherche, tapez Internet Explorer, puis dans la liste des résultats, cliquez sur **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="d7f5a-109">Cliquez sur **Outils**, puis sur **Options Internet**.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="d7f5a-110">Cliquez sur l’onglet **Sécurité**.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="d7f5a-111">Cliquez sur **sites intranet locaux** puis sur le bouton **sites**, puis le bouton **Avancé**.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="d7f5a-112">Entrez l’URL du site Web, puis cliquez sur **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="d7f5a-113">Lorsque vous avez terminé, cliquez sur **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="d7f5a-114">Pour plus d’informations, consulter [la documentation relative au déploiement de l’authentification unique transparente pour Office 365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inclut un processus basé sur des stratégies pour ajouter une URL aux sites intranet à l’étape 3).</span><span class="sxs-lookup"><span data-stu-id="d7f5a-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
