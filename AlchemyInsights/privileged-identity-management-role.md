---
title: Privileged Identity Management rôle
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973227"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**Les autorisations ne sont pas accordées après l’activation d’un rôle**

Lorsque vous activez un rôle dans Azure AD Privileged Identity Management (PIM), l’activation peut ne pas se propager instantanément à tous les portails qui nécessitent le rôle privilégié. Parfois, même si la modification est propagée, la mise en cache web dans un portail peut entraîner une non-prise d’effet immédiate de la modification.

Si votre activation est retardée, suivez les étapes suivantes :

1. Connectez-vous au portail Azure, puis connectez-vous. Lorsque vous activez un rôle Azure AD ou un rôle de ressource Azure, vous voyez les étapes de votre activation. Une fois toutes les étapes terminées, vous verrez un lien « Se terminer ». Vous pouvez utiliser ce lien pour vous mettre hors connexion. Cela permettra de résoudre la plupart des cas de retard d’activation.
2. Dans PIM, vérifiez que vous êtes répertorié en tant que membre du rôle.
3. Si vous activez le rôle d’Exchange, veillez à vous désinser et à vous y ré-inscrire. Si le problème persiste, ouvrez un ticket de support et ouvrez-le en tant que problème. Si vous utilisez votre rôle d Exchange pour accéder au Centre de sécurité et conformité, consultez l’étape suivante.
4. Si vous activez un rôle pour accéder au Centre de sécurité et conformité ou si vous activez le rôle d’administrateur SharePoint, vous pouvez connaître un certain délai d’activation de quelques minutes à quelques heures. Il s’agit d’un problème connu et nous travaillons activement avec ces équipes pour résoudre ce problème dès que possible.

Pour plus d’informations, voir :

- [Activer mes rôles Azure AD dans PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Activer mes rôles de ressources Azure dans PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Les autorisations ne sont pas supprimées après la désactivation d’un rôle ou l’activation du rôle expire**

Lorsque vous désactivez un rôle dans Azure AD Privileged Identity Management ou à l’expiration d’une période d’activation de rôle, il peut y avoir un délai dans lequel vous continuez d’avoir accès.

Si votre désactivation est retardée, suivez les étapes suivantes :

1. Si vous désactivez le rôle administrateur Exchange ou que la période d’activation du rôle expire et que vous remarquez un retard important avant la suppression des autorisations, ouvrez un ticket de support et indiquez à votre ingénieur du support technique de vous aider à déposer un ticket auprès de l’équipe pam (Privileged Access Management) au sein de Office à propos de ce problème.
2. Si la période d’activation a expiré, mais que la session du navigateur est toujours ouverte, fermez votre navigateur. Vous pouvez continuer à utiliser le rôle jusqu’à la fermeture de cette session. This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.

Si votre délai est différent de ces deux scénarios, ouvrez un ticket de support.
