---
title: Envoyer un message électronique en fournissant l’ID de message réseau
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735884"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Envoyer un message électronique en fournissant l’ID de message réseau

1. Dans le **volant Nouvelle soumission,** sélectionnez **E-mail** et **ID de message réseau.**
2. Suivez ces étapes pour rechercher l’ID de message d’un message électronique dans Outlook :
    1. Double-cliquez sur le message électronique pour l’ouvrir.
    1. Sélectionnez **les**  >  **propriétés du fichier.**
    1. Ouvrez le Bloc-notes ou un document Word vide, puis copiez et collez le contenu trouvé dans la zone d’en-tête **Internet** dans le document ouvert pour une meilleure visibilité.
    1. Recherchez **le champ X-MS-Exchange-Organization-Network-Message-Id.** La valeur après **:** est l’ID dont vous avez besoin pour votre soumission.
3. Sous **Destinataires**, si le courrier électronique a été envoyé dans le dossier courrier indésirable pour tous les destinataires de ce message, sélectionnez **Sélectionner tout.** Si ce n’est pas le cas, sélectionnez uniquement l’utilisateur qui a signalé le problème.
4. Sous **Raison de l’envoi,** si vous sélectionnez Doit avoir été  **bloqué,** spécifiez si le message doit avoir été bloqué en tant que courrier **indésirable,** hameçonnage ou programme **malveillant,** puis sélectionnez **Envoyer.**

Pour plus d’informations, voir Comment soumettre des messages suspects de courrier indésirable, d’hameçonnage, d’URL et de fichiers [à Microsoft pour analyse.](https://go.microsoft.com/fwlink/?linkid=2101479)
