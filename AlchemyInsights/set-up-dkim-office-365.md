---
title: Configurer DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808705"
---
# <a name="setup-dkim"></a>Configurer DKIM

Les instructions complètes de configuration de DKIM pour les domaines personnalisés dans Microsoft 365 [sont les](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)mêmes.

1. Pour **chaque** domaine personnalisé, vous devez créer **deux** enregistrements CNAME DKIM au niveau du service d’hébergement DNS de votre domaine (généralement, le Bureau d’enregistrement de domaines). Par exemple, contoso.com et fourthcoffee.com requièrent quatre enregistrements CNAMe DKIM : deux pour contoso.com et deux pour fourthcoffee.com.

   Les enregistrements CNAMe DKIM pour **chaque** domaine personnalisé utilisent les formats suivants :

   - **Nom**de l’hôte : `selector1._domainkey.<CustomDomain>`

     **Pointe vers l’adresse ou la valeur**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nom**de l’hôte : `selector2._domainkey.<CustomDomain>`

     **Pointe vers l’adresse ou la valeur**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> est le texte à gauche de `.mail.protection.outlook.com` dans l’enregistrement MX personnalisé pour le domaine personnalisé (par exemple, `contoso-com` pour le domaine contoso.com). \<InitialDomain\> est le domaine que vous avez utilisé lorsque vous vous êtes inscrit à Microsoft 365 (par exemple, contoso.onmicrosoft.com).

2. Une fois que vous avez créé les enregistrements CNAMe pour vos domaines personnalisés, procédez comme suit :

   a. [Connectez-vous à Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) avec votre compte professionnel ou scolaire.

   b. Sélectionnez l’icône du lanceur d’applications située en haut à gauche et choisissez **Administrateur**.

   c. Dans le volet de navigation en bas à gauche, développez **Administrateur** et choisissez **Exchange**.

   d. Accédez à **protection**  >  **DKIM**.

   e. Sélectionnez le domaine, puis sélectionnez **activer** pour **signer les messages pour ce domaine avec des signatures DKIM**. Répétez cette étape pour chaque domaine personnalisé.
