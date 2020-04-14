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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241250"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Corriger les messages bloqués dans la boîte d’envoi

Nous vous recommandons de commencer par exécuter le scénario [« je rencontre des problèmes lors de l’envoi, de la réception ou de la recherche de messages électroniques »](https://aka.ms/SaRA-OutlookSendReceive) à partir de l’outil de [support et de récupération Microsoft](https://diagnostics.office.com/#/) .

Lorsqu’un message est bloqué dans votre boîte d’envoi, la cause la plus probable est une pièce jointe de grande taille ou l’option « envoyer immédiatement une fois connecté » n’est pas activée.

**Supprimer la pièce jointe de grande taille**

1. Dans Outlook **, sélectionnez** > **travailler en mode hors connexion**. 
2. Dans le volet de navigation, sélectionnez **boîte d’envoi**. À partir de là, vous pouvez : 
    - Supprimez le message (sélectionnez-le, puis sélectionnez **supprimer**).
    - Faites glisser le message vers votre dossier Brouillons, double-cliquez dessus pour l’ouvrir, puis supprimez la pièce jointe sélectionnez-la, puis sélectionnez **supprimer**).
3. Si vous recevez une erreur indiquant qu’Outlook tente de transmettre le message, fermez Outlook. La fermeture peut prendre quelques instants. Si Outlook ne se ferme pas, appuyez sur CTRL + ALT + SUPPR et sélectionnez **Démarrer le gestionnaire des tâches**. Dans le gestionnaire des tâches, sélectionnez l’onglet **processus** , faites défiler vers le bas jusqu’à Outlook. exe et sélectionnez **terminer le processus**.
4. Après avoir fermé Outlook, redémarrez-le et répétez les étapes 2 et 3. 
5. Après avoir supprimé la pièce jointe **, cliquez sur** > **travailler en mode hors connexion** pour reprendre votre travail en ligne. 

Les messages sont également bloqués dans la boîte d’envoi lorsque vous cliquez sur **Envoyer**, mais vous n’êtes pas connecté. Cliquez sur **Envoyer/recevoir** , puis examinez le bouton **travailler hors connexion** . S’il est bleu, c’est que vous êtes déconnecté. Cliquez dessus pour vous connecter (le bouton active le blanc), puis cliquez sur **envoyer tout**.
 
**Activer l’envoi immédiat une fois connecté**
 
1. Sous l’onglet Fichier, cliquez sur **Options**.

2. Dans la boîte de dialogue Options d’Outlook, cliquez sur **Options avancées**.

3. Dans la section envoyer et recevoir, cliquez sur pour activer l' **envoi immédiat une fois connecté**. Cliquez sur **OK**.
 
Pour plus d’informations, reportez-vous à :
- [Vidéo : envoyer ou supprimer un e-mail bloqué](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Le courrier électronique reste dans le dossier boîte d’envoi tant que vous n’avez pas lancé manuellement une opération d’envoi/réception dans Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
