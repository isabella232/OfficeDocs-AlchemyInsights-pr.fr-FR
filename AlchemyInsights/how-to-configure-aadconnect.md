---
title: 646 comment configurer AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 316d7253494c55a9bc94797d493897c2ddec516c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541583"
---
# <a name="configure-sync-features"></a><span data-ttu-id="ecdc8-102">Configurer les fonctionnalités de synchronisation</span><span class="sxs-lookup"><span data-stu-id="ecdc8-102">Configure sync features</span></span>

<span data-ttu-id="ecdc8-103">Azure AD Connect comprend plusieurs fonctionnalités qui sont activées par défaut ou que vous pouvez activer ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="ecdc8-104">Certaines fonctionnalités nécessitent une configuration supplémentaire dans des environnements spécifiques.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="ecdc8-105">Limites de [filtrage](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) les objets sont synchronisés avec Azure ad.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="ecdc8-106">Par défaut, tous les utilisateurs, contacts, groupes et comptes d’ordinateur Windows 10 sont synchronisés.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="ecdc8-107">Vous pouvez inclure ou exclure des objets en fonction de domaines, d’unités d’organisation ou d’autres attributs.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="ecdc8-108">La [synchronisation de hachage de mot de passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronise le hachage de mot de passe de l’Active Directory local vers Azure ad.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="ecdc8-109">Cela permet de gérer les mots de passe à un seul emplacement, mais d’utiliser le même mot de passe dans les environnements locaux et Cloud.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="ecdc8-110">Étant donné qu’Active Directory est la source faisant autorité, vous pouvez utiliser vos propres stratégies de mot de passe.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="ecdc8-111">[Self-service Password Reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permet aux utilisateurs de réinitialiser leur mot de passe dans le Cloud tout en continuant à appliquer votre stratégie de mot de passe locale.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="ecdc8-112">L' [écriture différée du périphérique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permet de réécrire les appareils enregistrés dans Azure ad dans l’annuaire Active Directory local afin qu’ils puissent être utilisés pour l’accès conditionnel.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="ecdc8-113">[Empêcher](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) les suppressions accidentelles est activée par défaut pour empêcher trop de suppressions d’objets simultanées (plus de 500 objets par synchronisation).</span><span class="sxs-lookup"><span data-stu-id="ecdc8-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="ecdc8-114">Vous pouvez modifier ce paramètre pour répondre aux besoins de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="ecdc8-115">La [mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) est activée par défaut pour les installations rapides et garantit la mise à jour permanente de votre version d’Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="ecdc8-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
