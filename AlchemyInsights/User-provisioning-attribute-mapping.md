---
title: Mappage des attributs d’approvisionnement des utilisateurs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935363"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="26782-102">Mappage des attributs d’approvisionnement des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="26782-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="26782-103">Pour résoudre les problèmes connus de mappage des attributs, consultez [Mappages d’attributs](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="26782-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="26782-104">Microsoft Azure Active Directory (AD) fournit une assistance pour l’approvisionnement des utilisateurs vers des applications SaaS tierces telles que Salesforce, G Suite, etc.</span><span class="sxs-lookup"><span data-stu-id="26782-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="26782-105">Si vous activez l’approvisionnement des utilisateurs pour une application SaaS tierce, le portail Azure contrôle ses valeurs d’attribut à l’aide de mappages d’attributs.</span><span class="sxs-lookup"><span data-stu-id="26782-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="26782-106">Pour découvrir comment personnaliser les mappages d’attributs par défaut, consultez [Personnaliser les mappages d’attributs d’approvisionnement des utilisateurs pour les applications SaaS dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="26782-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="26782-107">Pour en savoir plus sur l’approvisionnement des utilisateurs de l’application SaaS, consultez [Qu’est-ce que l’approvisionnement automatique de l’application SaaS dans Azure AD ?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="26782-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="26782-108">Lors de la personnalisation des mappages d’attributs pour l’approvisionnement des utilisateurs, il est possible que l’attribut que vous voulez ma mappage n’apparaisse pas dans la liste des attributs source.</span><span class="sxs-lookup"><span data-stu-id="26782-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="26782-109">L’article [Synchroniser un attribut de votre Active Directory local vers Azure AD à des heures d’approvisionnement vers une application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) vous montre comment ajouter l’attribut manquant en le synchronisant à partir de votre AD local avec Azure AD.</span><span class="sxs-lookup"><span data-stu-id="26782-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
