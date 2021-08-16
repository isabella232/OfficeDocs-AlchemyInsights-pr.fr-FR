---
title: Rechercher l’adresse IP dans le journal d’audit
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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017130"
---
# <a name="find-the-ip-address-in-audit-log"></a>Rechercher l’adresse IP dans le journal d’audit

1. L’adresse IP qui correspond à une activité effectuée par un utilisateur ou un administrateur est affichée dans les journaux d’audit. Les informations client sont également enregistrées. Voici comment identifier l’adresse IP :

1. Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Sélectionnez **recherche**  >  **[dans le journal d’audit de recherche.](https://go.microsoft.com/fwlink/?linkid=2103759)**
    > [!NOTE]
    > Si vous voyez une notification vous avisant que vous devez activer l’audit, allez de l’avant et l’activer maintenant. Si cette fonctionnalité n’est pas activée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.
1. Si une activité spécifique vous intéresse, sélectionnez-la dans la liste **Activités** . Sinon, par défaut, toutes les activités sont renvoyées pour l’utilisateur sélectionné. Notez que certaines activités peuvent ne pas être disponibles pour la sélection dans le menu **Activités** ; toutefois, ces éléments d’audit sont renvoyés si **l’option Afficher** les résultats de toutes les activités est sélectionnée (paramètre par défaut).
1. Spécifiez la plage de dates et, dans le champ **Utilisateurs,** sélectionnez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner.
1. Sélectionner **Rechercher**. Les activités s’affichent sous **Résultats**. Vous pouvez voir l’adresse IP de chaque activité.
1. Pour afficher les détails, sélectionnez une activité, puis sélectionnez **Plus d’informations.**

Pour en savoir plus, consultez la Office 365 [journal d’audit pour résoudre les problèmes courants.](https://go.microsoft.com/fwlink/?linkid=2103944)