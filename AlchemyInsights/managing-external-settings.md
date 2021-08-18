---
title: Gestion des paramètres externes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: a988d792c51a81eac9aad3e8b2cd20fec9b2df51766f8919312e933a806e47ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114710"
---
# <a name="managing-external-settings"></a>Gestion des paramètres externes

**Annonce**

- [Prise en charge de la connexion à WebView depuis Google déconseillée à compter du 4 janvier 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support). Vérifiez si cela concerne vos applications en suivant les conseils de Google sur les tests de compatibilité
- Veillez à utiliser le système webview ou le navigateur système lorsque vous connectez à vos utilisateurs avec des comptes Google grand public

**Gérer les paramètres d’invitation**

Confirmez que vous avez [configuré les paramètres de collaboration externe](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) pour autoriser les personnes appropriées à envoyer des invitations.

**Gérer les autorisations d’accès des utilisateurs invités**

1. Les administrateurs globaux peuvent gérer les autorisations d’accès invité dans l’annuaire via le portail Azure en configurant les autorisations d’accès invité dans la page Paramètres de collaboration externe. [En savoir plus sur ce paramètre](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).
2. Si vous voulez que vos invités accèdent à des applications telles que Teams ou SharePoint, confirmez que vous les avez configurées pour autoriser l’accès invité. En savoir plus sur les [paramètres de Teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) et [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support) .

**Configuration d’invitations :**

- [Activer la collaboration externe B2B, puis gérer les utilisateurs pouvant avoir des invités](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Autoriser ou bloquer des invitations à des utilisateurs depuis des organisations spécifiques](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support).

**Configuration des fournisseurs d’identité autorisés :**

- [Fédération Google](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Fédération directe](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Authentification par envoi d’un code secret unique par e-mail](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
