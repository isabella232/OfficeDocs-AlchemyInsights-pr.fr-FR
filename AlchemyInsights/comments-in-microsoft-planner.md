---
title: Commentaires dans le planificateur Microsoft
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
- "9001717"
- "3810"
ms.openlocfilehash: 0d87d8c9fafe49de02b9c0158144287c77339886cdb910e006296eac73a2c497
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995504"
---
# <a name="comments-in-microsoft-planner"></a>Commentaires dans le planificateur Microsoft

Les commentaires relatifs à des tâches dans un plan sont stockés dans la boîte aux lettres Exchange Online pour le groupe Microsoft 365 associé au plan.  Lorsque vous publiez un commentaire sur une tâche, une notification par courrier électronique est envoyée à la boîte de réception du groupe. Vous recevrez un courrier électronique pour chaque commentaire ultérieur créé sur cette tâche.

Voici quelques réponses aux problèmes courants liés aux commentaires :

- **Les utilisateurs ne reçoivent pas de messages électroniques** : les commentaires sont envoyés à la boîte aux lettres du groupe auquel appartient le plan. Pour qu’un utilisateur puisse recevoir des messages de groupe, celui-ci doit être configuré pour envoyer les conversations de groupe vers les boîtes de réception des membres.

- **Les commentaires ne sont pas enregistrés** : l’utilisateur qui ajoute le commentaire n’est pas autorisé à envoyer des messages électroniques au groupe Microsoft 365. Pour plus d’informations sur ce scénario, consultez l’article[Fonctionnement du planificateur Microsoft](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736).

- L’erreur **vous n’avez plus d’accès** s’affiche, ou **Les utilisateurs invités ne peuvent pas ajouter de commentaires** : les utilisateurs invités qui ne peuvent pas envoyer de courrier électronique à la boîte aux lettres du groupe peuvent voir ce message. Pour résoudre ce problème, assurez-vous que l’utilisateur invité dispose d’une adresse e-mail valide.

- **Les utilisateurs supprimés reçoivent des courriers électroniques** : si un utilisateur ajoute une tâche avant d’être supprimé du plan, le fil de discussion de courrier électronique inclut l’utilisateur pour chaque commentaire créé sur la tâche.

Pour plus d’informations sur les commentaires à l’aide du planificateur Microsoft, consultez[Comment fonctionne le planificateur Microsoft](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) et [Ajouter des commentaires sur des tâches dans le planificateur Microsoft](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).
