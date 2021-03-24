---
title: Problèmes de certificat ou de secret client d’inscription de l’application
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123117"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problèmes de certificat ou de secret client d’inscription de l’application

La secret client de l’application arrive-t-elle à expiration ?

Quelle que soit la façon dont l’application enregistrée a été créée, que ce soit par le biais du processus d’inscription standard dans le portail d’inscription des applications ou si le principal de service a été créé dans votre client à l’aide du consentement de l’application, une nouvelle question secrète client doit être créée avant l’expiration de l’application actuelle et mise à jour dans le code d’application associé. La période de validité maximale est de 2 ans. Pour rappel, la valeur secrète doit être enregistrée, car elle n’est plus visible après avoir quitté la page Inscriptions de l’application dans le portail. Pour plus d’informations, voir [Démarrage rapide](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) : inscrire une application sur la plateforme d’identités Microsoft et meilleures pratiques pour la [plateforme d’identités Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Pour plus d’informations, voir Créer une application Azure AD & principal de service dans le [portail - Plateforme d’identités Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
