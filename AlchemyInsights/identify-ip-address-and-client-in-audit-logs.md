---
title: Identifier l’adresse IP et le client dans les journaux d’audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 080b3df3934781ebf0d0cd5243787bf6975fc5f123b5b1593c0b6d9ada4eae5d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887498"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifier l’adresse IP et le client dans les journaux d’audit

L’adresse IP qui correspond à une activité par un Microsoft 365 ou un administrateur est indiquée dans les journaux d’audit. Les informations client sont également enregistrées. Voici les étapes à suivre pour identifier ces informations

1. Connectez-vous au [Centre Microsoft 365 conformité.](https://protection.office.com/)

2. Go to the **Search**  >  **Audit log search** page.

   Si une activité spécifique vous intéresse, sélectionnez-la dans la liste **Activités.** Si ce n’est pas le cas, toutes les activités sont renvoyées pour l’utilisateur sélectionné (paramètre par défaut).

   **Remarque**: certaines activités peuvent ne pas être disponibles dans le menu **Activités** ; toutefois, ces éléments d’audit sont renvoyés si **l’option Afficher les** résultats pour toutes les activités est sélectionnée (paramètre par défaut).

3. Spécifiez le  nom d’utilisateur dans le champ Utilisateurs, sélectionnez la plage de dates appropriée pour l’activité, puis cliquez sur **Rechercher.**

Dans les résultats, vous pouvez voir l’adresse IP de cette activité dans le volet de résultats. Sélectionnez l’enregistrement d’audit pour voir des informations détaillées dans le volant **Détails** (par exemple, Client, Utilisateur qui a effectué une action, etc.).

Pour plus d’informations, [voir La recherche de l’adresse IP de l’ordinateur utilisé](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)pour accéder à un compte compromis.
