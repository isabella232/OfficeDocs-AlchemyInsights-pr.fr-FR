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
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011910"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Plusieurs objets ont la même adresse de courrier comme identité

**Objets multiples**

L’une des raisons les plus fréquentes de cette erreur est de ne pas pouvoir acheminer correctement une demande Outlook Web Access en présence de plusieurs objets ayant la même adresse de messagerie que l’identité. Pour rechercher ces objets, exécutez les commandes suivantes :

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