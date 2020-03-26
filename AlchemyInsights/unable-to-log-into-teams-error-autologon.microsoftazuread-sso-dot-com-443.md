---
title: Impossible de se connecter à Teams en raison d’une erreur autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931900"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Impossible de se connecter à Teams en raison d’une erreur autologon.microsoftazuread-sso dot com:443

Si l’authentification unique transparente est activée comme authentification Office 365, l’URL « autologon.microsoftazuread-sso.com » doit peut-être être ajoutée aux sites intranet.  Si elle a été précédemment ajoutée aux sites de confiance et que l’authentification unique transparente est utilisée, elle doit être supprimée des sites de confiance.

Consultez [la liste de contrôle pour la résolution des problèmes d’authentification unique transparente](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Pour ajouter une URL à la liste des sites intranet, procédez comme suit :

1. Pour ouvrir Internet Explorer, cliquez sur le bouton **démarrer**. Dans la zone de recherche, tapez Internet Explorer, puis dans la liste des résultats, cliquez sur **Internet Explorer**.
2. Cliquez sur **Outils**, puis sur **Options Internet**.
3. Cliquez sur l’onglet **Sécurité**.
4. Cliquez sur **sites intranet locaux** puis sur le bouton **sites**, puis le bouton **Avancé**.
5. Entrez l’URL du site Web, puis cliquez sur **Ajouter**.
6. Lorsque vous avez terminé, cliquez sur **Fermer**.

Pour plus d’informations, consulter [la documentation relative au déploiement de l’authentification unique transparente pour Office 365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inclut un processus basé sur des stratégies pour ajouter une URL aux sites intranet à l’étape 3).
