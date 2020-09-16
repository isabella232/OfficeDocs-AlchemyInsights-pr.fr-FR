---
title: Plusieurs objets ont la même adresse de courrier comme identité
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724613"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Plusieurs objets ont la même adresse de courrier comme identité

**Objets multiples**

L’une des raisons les plus fréquentes de cette erreur est de ne pas pouvoir acheminer correctement une demande Outlook Web Access en présence de plusieurs objets ayant la même adresse de messagerie que l’identité. Pour rechercher ces objets, exécutez les commandes suivantes :

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Pour résoudre le problème, supprimez plusieurs objets avec la même identité de courrier et assurez-vous qu’il existe un objet unique avec l’identité de courrier spécifique et que son type de destinataire est UserMailbox.

**La même adresse est utilisée pour les boîtes aux lettres d’entreprise et les boîtes aux lettres grand public**

Une autre cause est que la même adresse est utilisée pour les boîtes aux lettres d’entreprise et les boîtes aux lettres grand public. Dans ce cas, l’utilisateur doit changer d’alias de consommateur principal jusqu’à ce que le café prenne en charge ce scénario. Il s’agit d’une erreur permanente qui ne disparaît pas sans intervention.

Pour plus d’informations, consultez [Modifier l’adresse de courrier ou le numéro de téléphone de votre compte Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).