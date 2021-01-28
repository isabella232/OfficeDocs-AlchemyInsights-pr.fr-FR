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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="546a0-102">Problèmes avec les revendications et attributs de jeton</span><span class="sxs-lookup"><span data-stu-id="546a0-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="546a0-103">**Mettre à jour, configurer ou supprimer des revendications de jeton**</span><span class="sxs-lookup"><span data-stu-id="546a0-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="546a0-104">À l’aide d’Azure Active Directory (Azure AD), vous pouvez personnaliser le [type](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) de revendication pour la revendication de rôle dans le jeton de réponse que vous recevez après avoir autorisé une application.</span><span class="sxs-lookup"><span data-stu-id="546a0-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="546a0-105">Les développeurs d’applications peuvent utiliser des revendications facultatives dans leurs applications Azure AD pour spécifier les revendications qu’ils souhaitent dans les jetons envoyés à leur application.</span><span class="sxs-lookup"><span data-stu-id="546a0-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="546a0-106">Pour plus d’informations, [voir Fournir des revendications facultatives à votre application.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="546a0-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="546a0-107">[Configurez les revendications de groupe pour les applications avec Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="546a0-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="546a0-108">Si vous utilisez l' sign-on unique transparente dans votre application, voir personnaliser les revendications émises dans le jeton [SAML pour les applications d’entreprise.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="546a0-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="546a0-109">**Mappage des attributs de revendications**</span><span class="sxs-lookup"><span data-stu-id="546a0-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="546a0-110">Pour configurer la stratégie de mappage des revendications à l’aide de PowerShell, voir Personnaliser les revendications émises dans des jetons pour une application spécifique dans un [client (prévisualisation).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="546a0-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="546a0-111">Les attributs d’extension de schéma d’annuaire permettent de stocker des données supplémentaires dans Azure Active Directory sur des objets utilisateur et d’autres objets d’annuaire tels que des groupes, des détails client, des principaux de service.</span><span class="sxs-lookup"><span data-stu-id="546a0-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="546a0-112">Seuls les attributs d’extension sur les objets utilisateur peuvent être utilisés pour émettre des revendications vers des applications.</span><span class="sxs-lookup"><span data-stu-id="546a0-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="546a0-113">L’utilisation des [attributs d’extension](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) de schéma d’annuaire dans les revendications décrit comment utiliser les attributs d’extension de schéma d’annuaire pour envoyer des données utilisateur à des applications dans des revendications de jeton.</span><span class="sxs-lookup"><span data-stu-id="546a0-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="546a0-114">Pour plus d’informations sur les revendications de jeton, voir :</span><span class="sxs-lookup"><span data-stu-id="546a0-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="546a0-115">Revendications dans les jetons d’accès</span><span class="sxs-lookup"><span data-stu-id="546a0-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="546a0-116">Revendications dans une id_token</span><span class="sxs-lookup"><span data-stu-id="546a0-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="546a0-117">[Revendications que](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) vous pouvez attendre dans les jetons d’ID et les jetons d’accès émis par Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="546a0-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="546a0-118">Référence des revendications de jeton SAML</span><span class="sxs-lookup"><span data-stu-id="546a0-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
