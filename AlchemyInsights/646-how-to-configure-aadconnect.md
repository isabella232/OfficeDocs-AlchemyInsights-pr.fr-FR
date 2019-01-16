---
title: 646 comment configurer AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287883"
---
# <a name="configure-sync-features"></a><span data-ttu-id="fff30-102">Configurer les fonctionnalités de synchronisation</span><span class="sxs-lookup"><span data-stu-id="fff30-102">Configure sync features</span></span>

<span data-ttu-id="fff30-p101">Azure AD Connect inclut plusieurs fonctionnalités qui sont activées par défaut, ou que vous pouvez activer ultérieurement. Certaines fonctionnalités nécessitent une configuration supplémentaire dans des environnements spécifiques.</span><span class="sxs-lookup"><span data-stu-id="fff30-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="fff30-p102">Limites de [filtrage](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) les objets sont synchronisés avec Azure AD. Par défaut, tous les utilisateurs, contacts, groupes et Windows 10 comptes d’ordinateur sont synchronisées. Vous pouvez inclure ou exclure des objets basés sur les domaines, unités d’organisation ou d’autres attributs.</span><span class="sxs-lookup"><span data-stu-id="fff30-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="fff30-p103">[Synchronisation de hachage de mot de passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronise le hachage de mot de passe à partir d’Active Directory local pour Azure AD. Cela permet de gestion des mots de passe dans un emplacement, mais l’utilisation du même mot de passe dans les deux locaux et environnements en nuage. Étant donné que Active Directory est la source d’autorité, vous pouvez utiliser vos propres stratégies de mot de passe.</span><span class="sxs-lookup"><span data-stu-id="fff30-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="fff30-111">[Mot de passe libre-service réinitialiser (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permet aux utilisateurs de réinitialiser leurs mots de passe dans le nuage tout en appliquant votre stratégie de mot de passe local.</span><span class="sxs-lookup"><span data-stu-id="fff30-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="fff30-112">[Écriture différée de périphériques](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permet aux périphériques inscrits dans Azure AD pour être réécrites dans Active Directory sur site afin qu’ils puissent être utilisées pour l’accès conditionnel.</span><span class="sxs-lookup"><span data-stu-id="fff30-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="fff30-p104">[Pas accidentelle de suppression](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) est activée par défaut pour empêcher les suppressions d’objets simultanées trop (plus de 500 objets par synchronisation). Vous pouvez modifier ce paramètre pour satisfaire les besoins de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="fff30-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="fff30-115">[Mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) est activée par défaut pour les installations express et contribue à garantit que votre version d’Azure AD Connect est toujours en cours.</span><span class="sxs-lookup"><span data-stu-id="fff30-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

