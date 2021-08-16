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
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025608"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Vous devez marquer un domaine ou un expéditeur de courrier comme sécurisé ?

- L’utilisation de **listes d’expéditeurs approuvés n’est pas recommandé** car elle ouvre votre organisation aux attaques d’usurpation d’identité, de hameçonnage et au courrier indésirable.
- Toutefois, s’il existe un besoin d’entreprise, nous vous **recommandons** l’utilisation de **[Règles de flux de courrier](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**. Nos recommandations garantissent l’authentification de l’expéditeur (vérification que le domaine expéditeur n’est pas usurpé). **Remarque** : nous vous déconseillons de gérer les faux positifs à l’aide de listes d’expéditeurs approuvés, car les exceptions au filtrage du courrier indésirable peuvent ouvrir votre organisation à des attaques au niveau de la sécurité. Si vos utilisateurs reçoivent des messages incorrectement marqués comme courrier indésirable, veuillez **[Signaler les messages et fichiers à Microsoft](https://protection.office.com/reportsubmission)**.
- Les expéditeurs sûrs dans Outlook, la liste des expéditeurs autorisés ou la liste des domaines autorisés dans les stratégies **anti-courrier indésirable doivent être évités** car les expéditeurs contournent toutes les protections contre le spam, l'usurpation d'identité et le hameçonnage, ainsi que l'authentification de l'expéditeur (SPF, DKIM, DMARC). Cette méthode ne doit être utilisée que pour des tests temporaires.
- La validation qu'un certain email a contourné l' évaluationanti-courrier indésirable peut être faite en vérifiant l'en-tête de message «X-Forefront-Antispam-Report» (SFV:SFE, SFV:SKA, SFV:SKN), voir **[En-têtes de message anti-courrier indésirable](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.
- Parce que Microsoft veut que ses clients soient [sécurisés par défaut](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions), certaines dérogations des locataires ne sont pas appliquées pour les logiciels malveillants et le hameçonnage à haut degré de confiance. Ces remplacements comprennent : o Listes d'expéditeurs autorisés ou listes de domaines autorisés ( stratégies anti-courrier indésirable) o Expéditeurs sûrs d'Outlook o Liste d'IP autorisés (filtrage de connexion) 
- Les règles de flux de courrier d'Exchange (également connues sous le nom de règles de transport) sont les seules à permettre aux messages de hameçonnage de haute confiance de contourner le filtrage. Pour utiliser les règles de flux de courrier afin de contourner le filtrage, voir **[Utiliser les règles de flux de courrier pour définir le niveau de confiance du spam (SCL) dans les messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.