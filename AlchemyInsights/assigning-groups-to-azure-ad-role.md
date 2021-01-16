---
title: Attribution de groupes au rôle Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875365"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Attribution de groupes au rôle Azure AD

Pour attribuer un groupe Azure AD ayant la source d’autorité dans Azure AD à un rôle Azure AD, effectuez ces étapes :

1. Créer un groupe : Pour créer un groupe :

    a. Connectez-vous au centre d’administration Azure AD avec des autorisations **d’administrateur de rôle privilégié** ou **d’administrateur général**.
    b. Sélectionnez **Azure Active Directory > Groupes > Tous les groupes > Nouveau groupe**.
    c. Créer le groupe.

2. Attribuez le rôle au groupe lors de la création du groupe ou après la création du groupe.

    a. Pour attribuer un rôle au groupe au moment de la création du groupe, basculez sur le bouton bascule **Des rôles Azure AD peuvent être attribués au groupe**, puis créer le groupe.
    b. Pour attribuer un rôle au groupe après sa création, accédez à l’onglet **Rôles attribués** du nouveau groupe, puis attribuez le rôle au groupe.  

**Gérer l’adhésion à un groupe affecté à un rôle Azure AD**

Pour empêcher l’élévation des privilèges, par défaut, seuls les administrateurs de rôles privilégiés et les administrateurs globaux peuvent modifier l’adhésion d’un groupe affecté à un rôle. Toutefois, ils peuvent choisir d’affecter un propriétaire à un tel groupe et déléguer cette tâche.

Pour plus de détails sur l’affectation de groupes cloud à des rôles Azure AD, consultez[Attribuer des rôles AD aux groupes cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Pour plus détails sur le dépannage des rôles attribués aux groupes cloud, consultez [Résoudre les problèmes liés aux rôles affectés aux groupes cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





