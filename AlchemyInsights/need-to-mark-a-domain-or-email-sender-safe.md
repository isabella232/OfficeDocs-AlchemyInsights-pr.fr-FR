---
title: Vous devez marquer un domaine ou un expéditeur de courrier comme sécurisé ?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803243"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Vous devez marquer un domaine ou un expéditeur de courrier comme sécurisé ?

- L’utilisation de **listes d’expéditeurs approuvés n’est pas recommandé** car elle ouvre votre organisation aux attaques d’usurpation d’identité, de hameçonnage et au courrier indésirable.
- Toutefois, s’il existe un besoin d’entreprise, nous vous **recommandons** l’utilisation de **[Règles de flux de courrier](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**. Nos recommandations garantissent l’authentification de l’expéditeur (vérification que le domaine expéditeur n’est pas usurpé). **Remarque** : nous vous déconseillons de gérer les faux positifs à l’aide de listes d’expéditeurs approuvés, car les exceptions au filtrage du courrier indésirable peuvent ouvrir votre organisation à des attaques au niveau de la sécurité. Si vos utilisateurs reçoivent des messages incorrectement marqués comme courrier indésirable, veuillez **[Signaler les messages et fichiers à Microsoft](https://protection.office.com/reportsubmission)**.
- Les expéditeurs approuvés dans Outlook, la liste des expéditeurs autorisés ou la liste de domaines autorisés dans les stratégies anti-courrier indésirable **doivent être évités** car les expéditeurs ignorent la protection contre le courrier indésirable, l’usurpation d’identité et l’authentification de l’expéditeur (SPF, DKIM, DMARC). Cette méthode est idéale pour les tests temporaires uniquement.
