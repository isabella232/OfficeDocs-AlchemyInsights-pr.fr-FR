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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232628"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Corriger les messages bloqués dans la boîte d’envoi

Nous vous recommandons de commencer par exécuter le scénario [« je rencontre des problèmes lors de l’envoi, de la réception ou de la recherche de messages électroniques »](https://aka.ms/SaRA-OutlookSendReceive) à partir de l’outil de [support et de récupération Microsoft](https://diagnostics.office.com/#/) sur l’ordinateur affecté.

Lorsqu’un message est bloqué dans votre boîte d’envoi, la cause la plus probable est une pièce jointe de grande taille ou l’option « envoyer immédiatement une fois connecté » n’est pas activée.

**Supprimer la pièce jointe de grande taille**

1.  > Cliquez **sur****travailler en mode hors connexion**. 
2. Dans le volet de navigation, cliquez sur **boîte d’envoi**. À partir de là, vous pouvez : 
    - Supprimez le message. Sélectionnez-le et cliquez sur **supprimer**.
    - Faites glisser le message vers votre **dossier Brouillons**, double-cliquez pour ouvrir le message et supprimez la pièce jointe (cliquez dessus, puis cliquez sur **supprimer**).
3. Si une erreur indique que Outlook tente de transmettre le message, fermez Outlook. La fermeture peut prendre quelques instants. Si Outlook ne se ferme pas, appuyez sur **Ctrl + Alt + Suppr** , puis cliquez sur **Démarrer le gestionnaire des tâches**. Dans le gestionnaire des tâches, sélectionnez l’onglet **processus** , faites défiler vers le bas jusqu’à Outlook. exe, puis cliquez sur **terminer le processus**.
4. Après avoir fermé Outlook, redémarrez Outlook et répétez les étapes 2-3. 
5. Après avoir supprimé la pièce jointe **, cliquez sur** > **travailler en mode hors connexion** pour désélectionner le bouton et continuer à travailler en ligne. 

Les messages sont également bloqués dans la boîte d’envoi lorsque vous cliquez sur **Envoyer**, mais vous n’êtes pas connecté. Cliquez sur **Envoyer/recevoir** , puis examinez le bouton **travailler hors connexion** . S’il est bleu, c’est que vous êtes déconnecté. Cliquez dessus pour vous connecter (le bouton active le blanc), puis cliquez sur **envoyer tout**.
 
**Activer l’envoi immédiat une fois connecté**
 
1. Sous l’onglet Fichier, cliquez sur **Options**.

2. Dans la boîte de dialogue Options d’Outlook, cliquez sur **Options avancées**.

3. Dans la section envoyer et recevoir, cliquez sur pour activer l' **envoi immédiat une fois connecté**. Cliquez sur **OK**.
 
Pour plus d’informations, reportez-vous à :
- [Vidéo : envoyer ou supprimer un e-mail bloqué](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Le courrier électronique reste dans le dossier boîte d’envoi tant que vous n’avez pas lancé manuellement une opération d’envoi/réception dans Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
