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
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="4fe17-102">Problèmes de certificat ou de secret client d’inscription de l’application</span><span class="sxs-lookup"><span data-stu-id="4fe17-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="4fe17-103">La secret client de l’application arrive-t-elle à expiration ?</span><span class="sxs-lookup"><span data-stu-id="4fe17-103">Application client secret expiring?</span></span>

<span data-ttu-id="4fe17-104">Quelle que soit la façon dont l’application enregistrée a été créée, que ce soit par le biais du processus d’inscription standard dans le portail d’inscription des applications ou si le principal de service a été créé dans votre client à l’aide du consentement de l’application, une nouvelle question secrète client doit être créée avant l’expiration de l’application actuelle et mise à jour dans le code d’application associé.</span><span class="sxs-lookup"><span data-stu-id="4fe17-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="4fe17-105">La période de validité maximale est de 2 ans.</span><span class="sxs-lookup"><span data-stu-id="4fe17-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="4fe17-106">Pour rappel, la valeur secrète doit être enregistrée, car elle n’est plus visible après avoir quitté la page Inscriptions de l’application dans le portail.</span><span class="sxs-lookup"><span data-stu-id="4fe17-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="4fe17-107">Pour plus d’informations, voir [Démarrage rapide](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) : inscrire une application sur la plateforme d’identités Microsoft et meilleures pratiques pour la [plateforme d’identités Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="4fe17-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="4fe17-108">Pour plus d’informations, voir Créer une application Azure AD & principal de service dans le [portail - Plateforme d’identités Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="4fe17-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
