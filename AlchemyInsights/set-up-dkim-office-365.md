---
title: Configuration de DKIM
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108554"
---
# <a name="setup-dkim"></a>Configuration de DKIM

Les instructions complètes pour configurer DKIM pour les domaines personnalisés Microsoft 365 [sont](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)ici.

1. Pour **chaque** domaine personnalisé, vous devez créer deux enregistrements **CNAME** DKIM au niveau du service d’hébergement DNS de votre domaine (généralement, le bureau d’enregistrement de domaines). Par exemple, les contoso.com et fourthcoffee.com nécessitent quatre enregistrements CNAME DKIM : deux pour contoso.com et deux pour fourthcoffee.com.

   Les enregistrements CNAME DKIM pour **chaque** domaine personnalisé utilisent les formats suivants :

   - **Nom d’hôte**: `selector1._domainkey.<CustomDomain>`

     **Pointe vers l’adresse ou la valeur**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nom d’hôte**: `selector2._domainkey.<CustomDomain>`

     **Pointe vers l’adresse ou la valeur**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> est le texte à gauche de l’enregistrement MX personnalisé pour le domaine personnalisé (par exemple, pour le domaine `.mail.protection.outlook.com` `contoso-com` contoso.com). \<InitialDomain\>est le domaine que vous avez utilisé lorsque vous vous êtes inscrit à Microsoft 365 (par exemple, contoso.onmicrosoft.com).

2. Une fois que vous avez créé les enregistrements CNAME pour vos domaines personnalisés, complétez les instructions suivantes :

   a. [connectez-vous Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) avec votre compte scolaire ou scolaire.

   b. Sélectionnez l’icône du lanceur d’applications située en haut à gauche et choisissez **Administrateur**.

   c. Dans le volet de navigation en bas à gauche, développez **Administrateur** et choisissez **Exchange**.

   d. Go to **Protection**  >  **DKIM**.

   e. Sélectionnez le domaine, puis choisissez **Activer** pour **les messages de signature pour ce domaine avec des signatures DKIM.** Répétez cette étape pour chaque domaine personnalisé.
