---
title: Identification de l’adresse IP et du client dans les journaux d’audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539027"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identification de l’adresse IP et du client dans les journaux d’audit

L’adresse IP qui correspond à une activité par un utilisateur ou un administrateur Office 365 est affichée dans les journaux d’audit. Les informations sur le client sont également consignées. Voici les étapes à suivre pour identifier ces informations

1. Connectez-vous au [Centre de sécurité & conformité Office 365](https://protection.office.com/).

2. Accédez à la page de**recherche du journal d’audit** de la **recherche** > .

   Si vous êtes intéressé par une activité spécifique, sélectionnez-la dans la liste **activités** . Si ce n’est pas le cas, toutes les activités seront retournées pour l’utilisateur sélectionné (paramètre par défaut).

   **Remarque**: certaines activités ne sont pas disponibles dans le menu **activités** ; Toutefois, ces éléments d’audit seront renvoyés si l’option **afficher les résultats de toutes les activités** est sélectionnée (paramètre par défaut).

3. Spécifiez le nom d’utilisateur dans le champ **utilisateurs** , sélectionnez la plage de dates appropriée pour l’activité, puis cliquez sur **Rechercher**.

Dans les résultats, vous pouvez voir l’adresse IP de cette activité dans le volet de résultats. Sélectionnez l’enregistrement d’audit pour afficher des informations détaillées dans la fenêtre mobile des **Détails** (par exemple, le client, l’utilisateur qui a effectué l’action, etc.).

Pour plus d’informations, consultez [la rubrique recherche de l’adresse IP de l’ordinateur utilisé pour accéder à un compte compromis](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
