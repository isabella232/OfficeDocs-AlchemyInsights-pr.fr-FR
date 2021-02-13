---
title: Synchronisation du hachage de mot de passe pour service de domaine.
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162923"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="14345-102">Synchronisation du hachage de mot de passe pour service de domaine.</span><span class="sxs-lookup"><span data-stu-id="14345-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="14345-103">**Si votre instance Azure AD DS vous invite à activer la synchronisation du hachage de mot de passe**</span><span class="sxs-lookup"><span data-stu-id="14345-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="14345-104">Vous êtes dans un scénario d’exécution d’un environnement hybride avec une synchronisation d’utilisateurs depuis un environnement Azure Active Directory Domain Services (AD DS) local.</span><span class="sxs-lookup"><span data-stu-id="14345-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="14345-105">Ce scénario se produit malgré la synchronisation du hachage de mot de passe de l’environnement AD DS local à votre client Azure AD.</span><span class="sxs-lookup"><span data-stu-id="14345-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="14345-106">**Cause**</span><span class="sxs-lookup"><span data-stu-id="14345-106">**Cause**</span></span>

<span data-ttu-id="14345-107">Ce scénario se produit, car Azure AD Connect par défaut ne synchronise pas les hachages de mot de passe hérités New Technology LAN Manager (NTLM) et Kerberos nécessaires pour Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="14345-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="14345-108">**Solution de contournement**</span><span class="sxs-lookup"><span data-stu-id="14345-108">**Workaround**</span></span> 

<span data-ttu-id="14345-109">Vous devez configurer Azure AD Connect pour synchroniser les hachages de mot de passe requis pour l’authentification NTLM et Kerberos.</span><span class="sxs-lookup"><span data-stu-id="14345-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="14345-110">Une fois Azure AD Connect configuré, un événement de modification de mot de passe ou de création de compte local synchronise alors également les hachages du mot de passe hérité avec Azure AD.</span><span class="sxs-lookup"><span data-stu-id="14345-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="14345-111">Si vous souhaitez en savoir plus à ce sujet et sur l’activation de la synchronisation des mots de passe dans les environnements hybrides Azure AD DS, veuillez consulter [cette rubrique](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync).</span><span class="sxs-lookup"><span data-stu-id="14345-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>