---
title: Résoudre les problèmes de SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428694"
---
# <a name="troubleshoot-sspr"></a>Résoudre les problèmes de SSPR

**J’ai des difficultés à configurer la réinitialisation du mot de passe**

- Si vous êtes administrateur et que vous cherchez à activer la réinitialisation du mot de passe en libre-service, voir didacticiel activer [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), pour configurer la réinitialisation de mot de passe pour votre organisation. Vous pouvez également examiner les exigences de [licence.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Vous devez avoir au moins une licence attribuée dans votre organisation.
    - **Utilisateurs cloud uniquement** : toute référence (SKU) payante Office 365 (O365) ou Azure AD Basic
    - **Utilisateurs cloud et/ou** locaux : Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
- Pour d’autres questions sur la réinitialisation du mot de passe en libre-service, [lisez notre FAQ.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Je vois un message d’erreur**

Examinez cet article pour rechercher les erreurs courantes et leurs solutions : résoudre les problèmes de réinitialisation du mot [de passe en libre-service](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**J’ai un problème avec ma stratégie de réinitialisation de mot de passe**

- Si votre stratégie de réinitialisation de mot de passe ne se comporte pas comme prévu, ou si vous avez des questions sur les stratégies de réinitialisation de mot de passe, lisez cet article : Stratégies et restrictions de mot de passe dans [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Les stratégies de réinitialisation de mot de passe ne s’appliquent pas aux administrateurs. Microsoft applique une stratégie de réinitialisation de mot de passe à deux portails par défaut pour tout rôle d’administrateur Azure. Assurez-vous que vous testez avec un utilisateur qui n’est pas administrateur. Pour plus d’informations sur la stratégie de réinitialisation de l’administrateur, consultez cet article : Différences de stratégie de [réinitialisation de l’administrateur.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Je ne souhaite pas que mes utilisateurs enregistrent des informations de sécurité supplémentaires pour la réinitialisation du mot de passe**

Vous pouvez pré-remplir les données (attributs de messagerie et de téléphone) de vos utilisateurs à l’aide d’une API, de PowerShell ou d’Azure AD Connect. Pour savoir comment lire :

- [Déploiement de la réinitialisation du mot de passe sans obliger les utilisateurs à s’inscrire](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Données utilisées par la réinitialisation du mot de passe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Je souhaite que mes utilisateurs enregistrent leurs informations de sécurité supplémentaires pour la réinitialisation du mot de passe**

1. Demande à vos utilisateurs d’inscrire leurs informations de sécurité pour réinitialiser le mot de passe en libre-service en [les](https://mysignins.microsoft.com/security-info)aka.ms/ssprsetup .
1. Une fois que les données sont remplies pour l’utilisateur (par l’utilisateur ou par l’administrateur), [dirigez](https://passwordreset.microsoftonline.com/) votre utilisateur vers aka.ms/sspr afin que vos utilisateurs soient habilités à réinitialiser leurs propres mots de passe.
1. Si les utilisateurs rencontrent encore  des problèmes, ils sont très probablement des utilisateurs fédérés ou de hachage de mot de passe **synchronisés.** Cela signifie qu’il y a probablement un problème avec le service d’écriture écriture par mot de passe.