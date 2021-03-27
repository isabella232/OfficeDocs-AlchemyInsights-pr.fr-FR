---
title: Autorisations d’API et processus de consentement
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379829"
---
# <a name="api-permissions-and-consent-process"></a>Autorisations d’API et processus de consentement

Pour que votre application puisse accéder aux données dans Microsoft Graph, l’utilisateur ou l’administrateur doivent lui accorder les autorisations appropriées via un processus de consentement. [La référence des autorisations Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) répertorie les autorisations associées à chaque ensemble majeur d’API Microsoft Graph. Elle fournit également des instructions sur l’utilisation des autorisations.

**Configurer ou mettre à jour le principal de service**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) : cet article vous montre comment créer un objet servicePrincipal.
- Créez un principal de service d’application [Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) dans le portail : cet article vous montre comment créer une application Azure Active Directory (Azure AD) et un principal de service qui peuvent être utilisés avec le contrôle d’accès basé sur les rôles.
- Applications & principaux de service dans [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - Cet article décrit l’inscription des applications, les objets d’application et les principaux de service dans Azure Active Directory : ce qu’ils sont, comment ils sont utilisés et comment ils sont liés les uns aux autres.

**Ajouter ou mettre à jour l’inscription de l’application et fournir le consentement de l’administrateur**

- [Créer une inscription d’application](https://docs.microsoft.com/graph/api/application-post-applications) : cet article vous montre comment créer un objet d’application.
- [Mettre à jour l’inscription d’une application - Autorisations d’API](https://docs.microsoft.com/graph/api/application-update) - Cet article vous montre comment mettre à jour les propriétés d’un objet d’application.
- [Fournir le consentement de l’administrateur](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) : pour le consentement et le consentement de l’administrateur en général, nous exigeons qu’un administrateur donne explicitement son consentement.
- [RBAC (bêta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) : conteneur de gestion des rôles pour les définitions de rôle unifiées et les attributions de rôles pour les fournisseurs RBAC Microsoft 365 qui utilisent plusieurs principaux et plusieurs étendues dans une seule attribution de rôle. Il est différent du type de *ressource rbacApplication.* Microsoft Intune est un exemple de fournisseur RBAC de ce type. Une attribution de rôle dans Intune peut avoir un tableau de principaux et un tableau de groupes d’étendues. **Il s’agit de la version bêta, ce qui signifie qu’elle est toujours en développement et qu’elle n’est pas recommandée pour une utilisation en production.**
