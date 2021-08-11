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
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951491"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problèmes de certificat ou de secret client d’inscription de l’application

La secret client de l’application arrive-t-elle à expiration ?

Quelle que soit la façon dont l’application inscrite a été créée, que ce soit par le biais du processus d’inscription standard dans le portail d’inscription des applications ou si le principal de service a été créé dans votre client à l’aide du consentement de l’application, une nouvelle question secrète client doit être créée avant l’expiration de l’application actuelle et mise à jour dans le code d’application associé. La période de validité maximale est de 2 ans. Pour rappel, la valeur secrète doit être enregistrée, car elle ne sera plus visible après avoir quitté la page Inscriptions de l’application dans le portail. Pour plus d’informations, voir [Démarrage rapide](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) : inscrire une application dans le Plateforme d’identités Microsoft et meilleures pratiques pour [le Plateforme d’identités Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Pour plus d’informations, voir Créer une [application Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)& principal de service dans le portail - Plateforme d’identités Microsoft .
