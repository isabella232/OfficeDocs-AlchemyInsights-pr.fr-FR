---
title: Savoir qui a installé le forwarding sur une boîte aux lettres et comment
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988197"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Savoir qui a installé le forwarding sur une boîte aux lettres et comment

Si le forwarding externe a été définie sur une boîte aux lettres, l’activité est auditée dans le cadre Set-Mailbox cmdlet. Voici comment rechercher l’activité dans le journal d’audit :

1. Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Sélectionnez **recherche** >  **dans le journal d’audit de recherche.**
    > [!NOTE]
    > Si vous voyez une notification vous avisant que vous devez activer l’audit, allez de l’avant et l’activer maintenant. Si cette fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.
1. Assurez-vous **que le champ Activités** est définie sur Afficher les résultats pour toutes les **activités** (valeur par défaut). Spécifiez la plage de dates. Vous n’avez pas besoin de spécifier un nom d’utilisateur.
1. Sélectionner **Rechercher**. Les activités s’affichent sous **Résultats**.
1. Sélectionnez **Résultats du** filtre, puis entrez **Set-mailbox** dans le champ **De** filtre Activité. Cette action renvoie toutes **les activités Set-Mailbox.**
1. Pour afficher les détails, sélectionnez une activité, puis sélectionnez **Plus d’informations.** Sous **Paramètres,** vous pouvez voir l’adresse de messagerie de forwarding qui a été définie sur la boîte aux lettres. UserID **représente** l’utilisateur qui a installé le forwarding externe sur la boîte aux lettres.
Pour plus d’informations, consultez la Office 365 [d’audit pour résoudre les problèmes courants.](https://go.microsoft.com/fwlink/?linkid=2103944)