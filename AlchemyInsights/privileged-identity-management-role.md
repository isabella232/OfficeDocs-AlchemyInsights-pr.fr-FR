---
title: Rôle de gestion des identités privilégiées
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086284"
---
# <a name="privileged-identity-managementpim-role"></a>Rôle de gestion des identités avec privilèges (PIM)

**Les autorisations ne sont pas accordées après l’activation d’un rôle**

Lorsque vous activez un rôle dans Azure AD Privileged Identity Management (PIM), l’activation peut ne pas se propager instantanément à tous les portails qui nécessitent le rôle privilégié. Parfois, même si la modification est propagée, la mise en cache Web dans un portail peut empêcher le changement de prendre effet immédiatement.

Si votre activation est retardée, procédez comme suit :

1. Déconnectez-vous du portail Azure, puis reconnectez-vous. Lorsque vous activez un rôle Azure AD ou un rôle de ressource Azure, vous verrez les étapes de votre activation. Une fois toutes les étapes terminées, vous verrez un lien « Déconnexion ». Vous pouvez utiliser ce lien pour vous déconnecter. Cela permet de résoudre la plupart des cas de retard d’activation.
2. Dans le GIP, vérifiez que vous êtes répertorié en tant que membre du rôle.
3. Si vous activez le rôle Administrateur Exchange, assurez-vous de vous déconnecter et de vous reconnecter. Si le problème persiste, ouvrez un ticket de support et signalez-le comme un problème. Si vous utilisez votre rôle d’administrateur Exchange pour accéder au centre de sécurité et de conformité, reportez-vous à l’étape suivante.
4. Si vous activez un rôle pour accéder au centre de sécurité et de conformité ou si vous activez le rôle d’administrateur SharePoint, vous constaterez un certain délai d’activation de quelques minutes à quelques heures. Il s’agit d’un problème connu que nous collaborons activement avec ces équipes pour résoudre ce problème dès que possible.

Pour plus d’informations, reportez-vous aux rubriques suivantes :

- [Activer mes rôles Azure AD dans PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Activer mes rôles de ressource Azure dans PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Les autorisations ne sont pas supprimées après la désactivation d’un rôle ou l’activation de rôle expire**

Lorsque vous désactivez un rôle dans Azure AD Privileged Identity Management ou lorsqu’une période d’activation de rôle arrive à expiration, il se peut que vous continuiez à avoir accès.

Si votre désactivation est retardée, procédez comme suit :

1. Si vous désactivez le rôle d’administrateur Exchange ou que la période d’activation de rôle expire, et que vous remarquez un retard important avant la suppression des autorisations, ouvrez un ticket de support et indiquez à votre ingénieur de support de classer un ticket avec l’équipe PAM (Privileged Access Management) dans Office à propos de ce problème.
2. Si la période d’activation a expiré, mais que vous avez toujours ouvert la session de navigateur, fermez votre navigateur. Vous pouvez continuer à utiliser le rôle jusqu’à ce que vous fermiez cette session. Il s’agit d’un problème connu et nous examinons un correctif potentiel pour révoquer activement chaque session une fois l’activation expirée.

Si votre retard diffère de celui de ces deux scénarios, veuillez ouvrir un ticket de support.
