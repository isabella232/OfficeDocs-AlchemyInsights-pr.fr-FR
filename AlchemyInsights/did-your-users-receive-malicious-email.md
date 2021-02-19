---
title: Vos utilisateurs ont reçu des messages malveillants ?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291790"
---
# <a name="did-your-users-receive-malicious-email"></a>Vos utilisateurs ont reçu des messages malveillants ?

- Vous pouvez désormais signaler l’e-mail malveillant à Microsoft à l’aide des [soumissions d’administrateur dans le Centre de sécurité et de conformité](https://sip.protection.office.com/reportsubmission).

Le programme analyse les messages envoyés dans des soumissions [d'administrateur](https://sip.protection.office.com/reportsubmission), et les résultats suivants apparaissent dans le menu volant **Détails** :

- En cas d’échec de l’authentification des e-mails de l’expéditeur au moment de la livraison.
- Informations sur les accès à la stratégie qui auraient pu affecter ou écraser le verdict d’un message.
- Résultats actuels de la détonation pour savoir si les URL ou fichiers contenus dans le message étaient malveillants ou non.
- Commentaires des grilles d’évaluation

Si le programme a trouvé un remplacement, la nouvelle analyse doit se terminer après plusieurs minutes. Si le programme n’a pas rencontré de problème dans l’authentification d’e-mails ou si aucun remplacement n’a affecté la livraison, les commentaires des évaluateurs peuvent prendre jusqu’à un jour.

Si vous n’êtes pas d’accord avec le verdict sur un message, une URL ou un fichier (bloqué ou non), envoyez de nouveau le message après un jour pour nouvelle analyse. Le verdict a toutes les chances de changer après le nouvel envoi du message.

Pendant ce temps, vous pouvez supprimez les e-mails malveillants des boîtes de réception des utilisateurs en suivant les instructions de [cet article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Les clients qui disposent de Microsoft Defender pour Office 365 peuvent :
    - Utiliser l’[Explorateur de menaces pour rechercher, puis supprimer les e-mails suspects](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [utiliser la fonction Liens fiables pour bloquer l'accès](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) à une URL malveillante
    - suivre les utilisateurs qui ont cliqué sur des URL malveillantes, puis y ont accédé : [Afficher l’URL de phishing et cliquer sur les données du verdict](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - démarrer manuellement [une analyse automatisée](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Vous pouvez également vous protéger contre les fichiers et les URL malveillants en suivant les instructions fournies dans [Protection contre les URL et fichiers malveillants](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).