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
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952571"
---
# <a name="admin-consent-issues"></a>Problèmes de consentement de l’administrateur

1. Activez le [flux de travail de consentement de](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) l’administrateur pour permettre aux utilisateurs de demander l’approbation de l’administrateur directement à partir de l’écran de consentement.

1. Si vous ou les utilisateurs de votre application constatez des erreurs inattendues pendant le processus de consentement, consultez cet article pour les étapes de résolution des problèmes : [Erreur](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)inattendue lors de l’application du consentement.

1. En savoir plus sur le consentement de [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) l’administrateur [Plateforme d’identités Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)le fonctionnement de l’invite de consentement et l’évaluation d’une demande de consentement d’administrateur à l’échelle [du client.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Les applications qui s’intègrent Plateforme d’identités Microsoft suivent un modèle d’autorisation qui permet aux utilisateurs et aux administrateurs de contrôler la façon dont les données sont accessibles. L’implémentation du modèle d’autorisation a été mise à jour sur le point de terminaison Plateforme d’identités Microsoft et elle modifie la façon dont une application doit interagir avec le Plateforme d’identités Microsoft. Pour obtenir une vue d’ensemble de ce modèle d’autorisation, notamment les [étendues,](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) les autorisations et le consentement, voir autorisations et consentement dans le point de terminaison Plateforme d’identités Microsoft de l’utilisateur.