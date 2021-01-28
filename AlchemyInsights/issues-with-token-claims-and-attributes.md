---
title: Problèmes avec les revendications et attributs de jeton
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029980"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problèmes avec les revendications et attributs de jeton

**Mettre à jour, configurer ou supprimer des revendications de jeton**

1. À l’aide d’Azure Active Directory (Azure AD), vous pouvez personnaliser le [type](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) de revendication pour la revendication de rôle dans le jeton de réponse que vous recevez après avoir autorisé une application.
2. Les développeurs d’applications peuvent utiliser des revendications facultatives dans leurs applications Azure AD pour spécifier les revendications qu’ils souhaitent dans les jetons envoyés à leur application. Pour plus d’informations, [voir Fournir des revendications facultatives à votre application.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Configurez les revendications de groupe pour les applications avec Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Si vous utilisez l' sign-on unique transparente dans votre application, voir personnaliser les revendications émises dans le jeton [SAML pour les applications d’entreprise.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Mappage des attributs de revendications**

1. Pour configurer la stratégie de mappage des revendications à l’aide de PowerShell, voir Personnaliser les revendications émises dans des jetons pour une application spécifique dans un [client (prévisualisation).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Les attributs d’extension de schéma d’annuaire permettent de stocker des données supplémentaires dans Azure Active Directory sur des objets utilisateur et d’autres objets d’annuaire tels que des groupes, des détails client, des principaux de service. Seuls les attributs d’extension sur les objets utilisateur peuvent être utilisés pour émettre des revendications vers des applications. L’utilisation des [attributs d’extension](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) de schéma d’annuaire dans les revendications décrit comment utiliser les attributs d’extension de schéma d’annuaire pour envoyer des données utilisateur à des applications dans des revendications de jeton.

Pour plus d’informations sur les revendications de jeton, voir :

- [Revendications dans les jetons d’accès](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Revendications dans une id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Revendications que](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) vous pouvez attendre dans les jetons d’ID et les jetons d’accès émis par Azure AD B2C
- [Référence des revendications de jeton SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
