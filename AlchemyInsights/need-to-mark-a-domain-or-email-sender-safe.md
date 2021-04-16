---
title: Vous devez marquer un domaine ou un expéditeur de courrier comme sécurisé ?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792130"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Vous devez marquer un domaine ou un expéditeur de courrier comme sécurisé ?

- L’utilisation de **listes d’expéditeurs approuvés n’est pas recommandé** car elle ouvre votre organisation aux attaques d’usurpation d’identité, de hameçonnage et au courrier indésirable.
- Toutefois, s’il existe un besoin d’entreprise, nous vous **recommandons** l’utilisation de **[Règles de flux de courrier](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**. Nos recommandations garantissent l’authentification de l’expéditeur (vérification que le domaine expéditeur n’est pas usurpé). **Remarque** : nous vous déconseillons de gérer les faux positifs à l’aide de listes d’expéditeurs approuvés, car les exceptions au filtrage du courrier indésirable peuvent ouvrir votre organisation à des attaques au niveau de la sécurité. Si vos utilisateurs reçoivent des messages incorrectement marqués comme courrier indésirable, veuillez **[Signaler les messages et fichiers à Microsoft](https://protection.office.com/reportsubmission)**.
- Les expéditeurs approuvés dans Outlook, la liste des expéditeurs autorisés ou la liste de domaines autorisés dans les stratégies anti-courrier indésirable **doivent être évités** car les expéditeurs ignorent la protection contre le courrier indésirable, l’usurpation d’identité et l’authentification de l’expéditeur (SPF, DKIM, DMARC). Cette méthode est idéale pour les tests temporaires uniquement.
