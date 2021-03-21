---
title: Protection contre les attaques de rétrodiffusion
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897705"
---
# <a name="protection-from-backscatter-attack"></a>Protection contre les attaques de rétrodiffusion

La rétrodiffusion est les rapports d’erreur de remise (également appelés rapports d’erreur ou messages de non-remise) que vous recevez pour les messages que vous n’avez pas envoyés. Les expéditeurs de courrier indésirable falsifient (usurpent) l’adresse **De :** de leurs messages. Ils utilisent souvent des adresses de messagerie réelles pour donner de la crédibilité à leurs messages. Par conséquent, lorsque les expéditeurs de courrier indésirable envoient inévitablement des messages à des destinataires inexistants, le serveur de messagerie de destination est essentiellement piégé et renvoie le message non distribuable dans un NDR à l'expéditeur falsifié dans l'adresse **De :** .

Des informations supplémentaires sont disponibles dans la [Rétrodiffusion dans EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Activation de la protection contre la rétrodiffusion**

Pour activer la protection contre la rétrodiffusion, suivez le chemin d’accès ci-dessous.

**protection.office.com > Gestion des menaces > Stratégie > Anti-courrier indésirable > Sélectionner la stratégie de filtrage du courrier indésirable et modifier la stratégie > Propriétés du courrier indésirable > Marquer comme courrier indésirable > Rétrodiffusion NDR > Définir sur « Activé »**

Si vous pensez qu’un compte a été compromis, consultez ce qui suit :

- [Répondre à un compte d'e-mail compromis](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Suppression d’utilisateurs bloqués du portail Utilisateurs restreints dans Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



