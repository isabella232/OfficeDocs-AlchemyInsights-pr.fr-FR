---
title: Problèmes de consentement de l’administrateur
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888300"
---
# <a name="admin-consent-issues"></a>Problèmes de consentement de l’administrateur

1. Activez le [flux de travail de consentement de](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) l’administrateur pour permettre aux utilisateurs de demander l’approbation de l’administrateur directement à partir de l’écran de consentement.

1. Si vous ou les utilisateurs de votre application constatez des erreurs inattendues pendant le processus de consentement, consultez cet article pour les étapes de résolution des problèmes : [Erreur](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)inattendue lors de l’application du consentement.

1. En savoir plus sur le consentement de [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) l’administrateur sur la plateforme d’identité [Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)sur le fonctionnement de l’invite de consentement et sur l’évaluation d’une demande de consentement d’administrateur à l’échelle [du client.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Les applications qui s’intègrent à la plateforme d’identités Microsoft suivent un modèle d’autorisation qui permet aux utilisateurs et aux administrateurs de contrôler la façon dont les données sont accessibles. L’implémentation du modèle d’autorisation a été mise à jour sur le point de terminaison de la plateforme d’identités Microsoft et elle modifie la façon dont une application doit interagir avec la plateforme d’identités Microsoft. Voir [autorisations et consentement](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) dans le point de terminaison de la plateforme d’identités Microsoft pour obtenir une vue d’ensemble de ce modèle d’autorisation, y compris les étendues, les autorisations et le consentement.