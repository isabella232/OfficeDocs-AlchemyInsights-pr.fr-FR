---
title: Paramètres SMTP pour le service de messagerie Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107151"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Paramètres SMTP pour le service de messagerie Microsoft 365

Voici les paramètres SMTP pour le service de messagerie Microsoft 365

**Server** : smtp.office365.com </br>
**Port** : 587 </br>
**Chiffrement** : STARTTLS (Seule la version TLS 1.2 est prise en charge maintenant. Vérifiez que votre application ou appareil prend en charge TLS 1.2) </br>
**Nom d’utilisateur** : votre adresse Office 365 (par exemple, example@yourdomain.com) </br>
**Mot de passe** : votre mot de passe Office 365 </br>
**Authentification** : requise </br>
**Limites d’envoi** : 10 000 e-mails par jour </br>

Pour les paramètres POP et IMAP, consultez [Paramètres POP, IMAP et SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Pour en savoir plus sur vos options de relais de courrier électronique à l’aide de Microsoft 365 et des étapes, consultez [Comment configurer une application ou un périphérique multi-fonction pour envoyer des courriers électroniques à l’aide de Microsoft 365 ou Office 365](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)