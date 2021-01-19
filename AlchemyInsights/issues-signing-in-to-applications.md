---
title: Problème d’accès aux applications
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886850"
---
# <a name="issues-signing-in-to-applications"></a>Problème d’accès aux applications

Pour détecter la cause ou diagnostiquer les problèmes liés à la connexion de l’utilisateur, effectuez les étapes suivantes :

1. Lancez le [diagnostic de connexion](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Recherchez l’événement à analyser en entrant les détails dont vous avez besoin sur l’utilisateur, l’application, l’heure de la connexion, l’ID de demande ou l’ID de corrélation.
3. Examinez les résultats de diagnostic en indiquant les détails de ce qui s’est produit et les actions que vous pouvez prendre pour apporter des modifications, si des modifications sont nécessaires.

Voici quelques-uns des problèmes courants que vous pouvez éprouver lors de la connexion à des applications :

1. Vous ou l’utilisateur **avez effectué une connexion à Azure AD, mais une invite de commande inattendue s’affiche**. Consultez les articles [Invite de consentement inattendue lors de la connexion à une application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) et [Erreur inattendue lors de l’accord sur une application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Vous ou un utilisateur **vous êtes directement connecté à une application, mais vous ne pouvez pas vous y connecter à partir d’un lien approfondi sur le portail personnalisé ou le panneau d’accès**: Voir [Résoudre les problèmes de connexion à une application à partir d’Azure AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Vous ou un utilisateur **avez terminé une connexion à Azure AD, mais l’application affiche un message d’erreur et ne permet pas à l’utilisateur de terminer le processus de connexion** : le problème est que l’application n’a pas accepté la réponse qu’Azure AD a émise. Procédez[comme suit](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error)pour résoudre les erreurs.
4. Vous, ou un utilisateur **ne pouvez pas vous connecter à une application autre que la galerie configurée pour l’inscription unique par mot de passe**: suivez les instructions des[ étapes ](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) pour résoudre les problèmes.
5. Vous ou un utilisateur **ne pouvez pas vous connecter à une application autre que la galerie Azure AD configurée pour l’inscription unique par mot de passe**: suivez les instructions des[ étapes ](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) pour résoudre les problèmes.
6. Vous, ou un utilisateur **ne pouvez pas vous connectez à une application Microsoft**: suivez [ces étapes](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) pour résoudre les problèmes.
7. Vous ou un utilisateur **ne pouvez pas vous connecter à une application autre que la galerie configurée pour l’inscription unique fédérée**: suivez les instructions des[ étapes ](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) pour résoudre les problèmes.
8. Vous ou un utilisateur **ne pouvez pas vous connecter à une application autre que la galerie Azure AD configurée pour l’inscription unique fédérée**: suivez les instructions des[ étapes ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) pour résoudre les problèmes.
9. Vous, ou un utilisateur **ne pouvez pas vous connecter à une application Microsoft personnalisée**: suivez [ces étapes](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) pour résoudre les problèmes.
10. Vous, ou un utilisateur **ne pouvez pas vous connecter à une application en local à l’aide du proxy de l’application Azure AD** : Suivez ces [étapes](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) pour résoudre les problèmes.

