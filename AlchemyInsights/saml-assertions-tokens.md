---
title: Assertions SAML (jetons)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884588"
---
# <a name="saml-assertions-tokens"></a>Assertions SAML (jetons)

1. Les jetons SAML (Security Assertions Markup Language) sont des représentations XML des revendications. Par défaut, les jetons SAML que Windows Communication Foundation (WCF) utilise dans les scénarios de sécurité fédérée sont des jetons émis. Pour plus d’informations, [voir Jetons SAML et revendications.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. La plateforme d’identités Microsoft émet plusieurs types de jetons de sécurité dans le traitement de chaque flux d’authentification. [La référence des revendications de](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) jeton SAML décrit le format, les caractéristiques de sécurité et le contenu des jetons SAML 2.0.
3. Suivez les instructions de la plateforme d’identités Microsoft sur les durées de vie des jetons [configurables](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) pour comprendre comment configurer les durées de vie des jetons.
4. Suivez les étapes décrites dans [cet article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) pour comprendre comment configurer le chiffrement de jeton SAML Azure AD.
5. Dans Azure AD, vous pouvez configurer les options de signature de certificat et l’algorithme de signature de certificat. Pour plus d’informations, voir options avancées de signature de certificat dans le jeton SAML pour les applications de galerie [dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
