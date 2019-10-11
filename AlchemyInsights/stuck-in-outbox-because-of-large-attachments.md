---
title: Bloqué dans la boîte d’envoi en raison de pièces jointes volumineuses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441304"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Corriger les messages bloqués dans la boîte d’envoi

Nous vous recommandons de commencer par exécuter le scénario [« je rencontre des problèmes lors de l’envoi, de la réception ou de la recherche de messages électroniques »](https://aka.ms/SaRA-OutlookSendReceive) à partir de l’outil de [support et de récupération Microsoft](https://diagnostics.office.com/#/) .

Lorsqu’un message est bloqué dans votre boîte d’envoi, les causes les plus probables sont les suivantes :
- Pièces jointes volumineuses.
- L’option **Envoyer immédiatement une fois connecté** n’est pas activée.

Pour supprimer des pièces jointes volumineuses : 

1. Dans Outlook **, sélectionnez** > **travailler en mode hors connexion**. 
2. Dans le volet de navigation, sélectionnez **boîte d’envoi**. À partir de là, vous pouvez : 
    - Supprimez le message (sélectionnez-le, puis sélectionnez **supprimer**).
    - Faites glisser le message vers votre dossier Brouillons, double-cliquez dessus pour l’ouvrir, puis supprimez la pièce jointe sélectionnez-la, puis sélectionnez **supprimer**).
3. Si vous recevez une erreur indiquant qu’Outlook tente de transmettre le message, fermez Outlook. La fermeture peut prendre quelques instants. Si Outlook ne se ferme pas, appuyez sur CTRL + ALT + SUPPR et sélectionnez **Démarrer le gestionnaire des tâches**. Dans le gestionnaire des tâches, sélectionnez l’onglet **processus** , faites défiler vers le bas jusqu’à Outlook. exe et sélectionnez **terminer le processus**.
4. Après avoir fermé Outlook, redémarrez-le et répétez les étapes 2 et 3. 
5. Après avoir supprimé la pièce jointe **, cliquez sur** > **travailler en mode hors connexion** pour reprendre votre travail en ligne. 

Les messages sont également bloqués dans la boîte d’envoi lorsque vous cliquez sur **Envoyer**, mais vous n’êtes pas connecté. Cliquez sur **Envoyer/recevoir** , puis examinez le bouton **travailler hors connexion** . S’il est bleu, c’est que vous êtes déconnecté. Sélectionnez-le pour vous connecter (le bouton active le blanc), puis cliquez sur **envoyer tout**.
 
Pour activer l' **envoi immédiat une fois connecté**:
 
- Sélectionnez **** > **** options >  de fichier-**avancé**.
Dans la section **Envoyer et recevoir** , sélectionnez **Envoyer immédiatement une fois connecté**, puis choisissez **OK**.
 
Pour obtenir des informations complètes, voir :
- [Vidéo : envoyer ou supprimer un e-mail bloqué](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Le courrier électronique reste dans le dossier boîte d’envoi tant que vous n’avez pas lancé manuellement une opération d’envoi/réception dans Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
