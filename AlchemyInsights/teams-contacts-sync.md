---
title: Synchronisation des contacts de Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004610"
- "11540"
ms.openlocfilehash: 0ffa91f0e31a4904db87f0df6d9b4c51b05ae2758a5ce0d96c77ef4456f6d033
ms.sourcegitcommit: 71501cde5bcb73f4dcf23944d400a4db10f37033
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/09/2021
ms.locfileid: "57807186"
---
# <a name="teams-contacts-sync"></a>Synchronisation des contacts de Teams

Teams utilise les contacts de l’Active Directory de votre organisation, ainsi que les contacts ajoutés au dossier Outlook par défaut de l’utilisateur. Si les contacts ne s'affichent pas dans Microsoft Teams, essayez ce qui suit :

**Remarque :** si les informations d'un ou plusieurs contacts ont été récemment mises à jour, la synchronisation des contacts peut prendre jusqu'à 48 heures.

1. Déconnectez-vous de Teams et redémarrez. Vérifiez si vos contacts s'affichent.
1. Vider le cache Teams :
    1. Accédez à **%AppData%\Microsoft\Teams**.
    1. Supprimer le contenu du dossier
    1. Redémarrez l’ordinateur, puis lancez Teams.
1. Si le contact se trouve dans Outlook, veillez à l'ajouter à la liste des contacts. Dans Outlook, dans la barre d'adresse, sélectionnez **Fichier**, puis sélectionnez **Ajouter aux contacts**.
1. Assurez-vous que la boîte aux lettres Exchange de l'utilisateur est hébergée en ligne (et non sur site). Pour plus d’informations, voir [comment Exchange et Microsoft Teams interagissent](/microsoftteams/exchange-teams-interact).
1. Assurez-vous que le numéro de téléphone du contact est ajouté aux informations sur le contact.
1. Recherchez l’adresse e-mail du contact dans la barre de Recherche. Les contacts que vous pouvez récupérer sont synchronisés avec la Liste des contacts.
