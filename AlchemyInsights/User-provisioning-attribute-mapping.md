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
ms.openlocfilehash: 73da476cc5913a16911839a59b80959d3c99a8bc22471febe421b022ce2c49ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918141"
---
# <a name="user-provisioning-attribute-mapping"></a>Mappage des attributs d’approvisionnement des utilisateurs

1. Pour résoudre les problèmes connus de mappage des attributs, consultez [Mappages d’attributs](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) fournit une assistance pour l’approvisionnement des utilisateurs vers des applications SaaS tierces telles que Salesforce, G Suite, etc. Si vous activez l’approvisionnement des utilisateurs pour une application SaaS tierce, le portail Azure contrôle ses valeurs d’attribut à l’aide de mappages d’attributs. Pour découvrir comment personnaliser les mappages d’attributs par défaut, consultez [Personnaliser les mappages d’attributs d’approvisionnement des utilisateurs pour les applications SaaS dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Pour en savoir plus sur l’approvisionnement des utilisateurs de l’application SaaS, consultez [Qu’est-ce que l’approvisionnement automatique de l’application SaaS dans Azure AD ?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Lors de la personnalisation des mappages d’attributs pour l’approvisionnement des utilisateurs, il est possible que l’attribut que vous voulez ma mappage n’apparaisse pas dans la liste des attributs source. L’article [Synchroniser un attribut de votre Active Directory local vers Azure AD à des heures d’approvisionnement vers une application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) vous montre comment ajouter l’attribut manquant en le synchronisant à partir de votre AD local avec Azure AD.
