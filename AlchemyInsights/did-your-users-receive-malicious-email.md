---
title: Vos utilisateurs ont reçu des messages malveillants ?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326665"
---
# <a name="did-your-users-receive-malicious-email"></a>Vos utilisateurs ont reçu des messages malveillants ?

Vous pouvez désormais signaler l'e-mail malveillant à Microsoft Corporation en utilisant [la fonction Soumissions du portail Microsoft 365 Defender](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

Le programme analyse les messages envoyés dans des soumissions [d'administrateur](https://security.microsoft.com/reportsubmission?viewid=admin), et les résultats suivants apparaissent dans le menu volant Détails :

- En cas d’échec de l’authentification des e-mails de l’expéditeur au moment de la livraison.
- Informations sur les accès à la stratégie qui auraient pu affecter ou écraser le verdict d’un message.
- Résultats actuels de la détonation pour savoir si les URL ou fichiers contenus dans le message étaient malveillants ou non.
- Commentaires des grilles d’évaluation

Si une dérogation a été trouvée, le rescan devrait se terminer en quelques minutes. Si le programme n’a pas rencontré de problème dans l’authentification d’e-mails ou si aucun remplacement n’a affecté la livraison, les commentaires des évaluateurs peuvent prendre jusqu’à un jour.

Si vous n’êtes pas d’accord avec le verdict sur un message, une URL ou un fichier (bloqué ou non), envoyez de nouveau le message après un jour pour nouvelle analyse. Le verdict a toutes les chances de changer après le nouvel envoi du message.

Pendant ce temps, vous pouvez supprimez les e-mails malveillants des boîtes de réception des utilisateurs en suivant les instructions de [cet article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Les clients qui disposent de Microsoft Defender pour Office 365 peuvent :
  - Utiliser l’[Explorateur de menaces pour rechercher, puis supprimer les e-mails suspects](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Utiliser la fonction Liens fiables pour bloquer l'accès](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) à une URL malveillante
  - Suivre les utilisateurs qui ont cliqué sur des URL malveillantes, puis y ont accédé : [Afficher l’URL de phishing et cliquer sur les données du verdict](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Démarrer manuellement [une analyse automatisée](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Vous pouvez également vous protéger contre les fichiers et les URL malveillants en suivant les instructions fournies dans [Protection contre les URL et fichiers malveillants](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
