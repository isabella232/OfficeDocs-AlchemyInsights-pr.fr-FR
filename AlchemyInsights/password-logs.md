---
title: Journaux des mots de passe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523084"
---
# <a name="password-logs"></a><span data-ttu-id="4b3ef-102">Journaux des mots de passe</span><span class="sxs-lookup"><span data-stu-id="4b3ef-102">Password logs</span></span>

<span data-ttu-id="4b3ef-103">**J’ai des problèmes pour accéder aux journaux d’audit de réinitialisation du mot de passe**</span><span class="sxs-lookup"><span data-stu-id="4b3ef-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="4b3ef-104">Pour résoudre les problèmes de réinitialisation des mots de passe dans les journaux d’audit, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="4b3ef-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="4b3ef-105">Assurez-vous que vous êtes autorisé à afficher les journaux d’audit.</span><span class="sxs-lookup"><span data-stu-id="4b3ef-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="4b3ef-106">Seuls les rôles suivants sont autorisés :</span><span class="sxs-lookup"><span data-stu-id="4b3ef-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="4b3ef-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="4b3ef-107">Global administrator</span></span>
 - <span data-ttu-id="4b3ef-108">Administrateur de sécurité</span><span class="sxs-lookup"><span data-stu-id="4b3ef-108">Security administrator</span></span>
 - <span data-ttu-id="4b3ef-109">Lecteur Sécurité</span><span class="sxs-lookup"><span data-stu-id="4b3ef-109">Security reader</span></span>

<span data-ttu-id="4b3ef-110">**Je souhaite voir tous les événements d’audit de réinitialisation de mot de passe à partir du déploiement initial**</span><span class="sxs-lookup"><span data-stu-id="4b3ef-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="4b3ef-111">Jusqu’à 120 000 événements de réinitialisation/inscription de mot de passe sont stockés dans les rapports des 30 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="4b3ef-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="4b3ef-112">Cette limite maximale s’applique à l’interface utilisateur lors du téléchargement du fichier de valeurs séparées par des virgules.</span><span class="sxs-lookup"><span data-stu-id="4b3ef-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="4b3ef-113">Un million d’événements sont disponibles via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4b3ef-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="4b3ef-114">Pour plus d’informations, consultez les liens suivants :</span><span class="sxs-lookup"><span data-stu-id="4b3ef-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="4b3ef-115">Réinitialisation des événements de mot de passe libre-service à partir de l’API Rapports et événements Azure AD</span><span class="sxs-lookup"><span data-stu-id="4b3ef-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="4b3ef-116">Comment télécharger rapidement des événements d’inscription de réinitialisation de mot de passe avec PowerShell</span><span class="sxs-lookup"><span data-stu-id="4b3ef-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="4b3ef-117">**Je souhaite en savoir plus sur les fonctionnalités de réinitialisation de mot de passe**</span><span class="sxs-lookup"><span data-stu-id="4b3ef-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="4b3ef-118">Vérifiez qui s'inscrit ou réinitialise les mots de passe avec les journaux d'audit de réinitialisation des mots de passe Azure AD dans le Portail Azure sous **Utilisateurs et groupes**.</span><span class="sxs-lookup"><span data-stu-id="4b3ef-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="4b3ef-119">Pour plus d’informations, accédez aux liens suivants :</span><span class="sxs-lookup"><span data-stu-id="4b3ef-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="4b3ef-120">Vue d’ensemble des rapports de réinitialisation de mot de passe</span><span class="sxs-lookup"><span data-stu-id="4b3ef-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="4b3ef-121">Afficher les rapports de réinitialisation de mot de passe dans le Portail Azure</span><span class="sxs-lookup"><span data-stu-id="4b3ef-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="4b3ef-122">Réinitialisation des événements de mot de passe libre-service à partir de l’API Rapports et événements Azure AD</span><span class="sxs-lookup"><span data-stu-id="4b3ef-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="4b3ef-123">Comment télécharger rapidement des événements d’inscription de réinitialisation de mot de passe avec PowerShell</span><span class="sxs-lookup"><span data-stu-id="4b3ef-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


