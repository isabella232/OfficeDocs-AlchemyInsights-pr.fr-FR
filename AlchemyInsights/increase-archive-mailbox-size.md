---
title: 305 augmenter la taille de la boîte aux lettres d’archivage
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36661798"
---
# <a name="increase-the-archive-mailbox-size"></a>Augmenter la taille de la boîte aux lettres d’archivage

Office 365 [limite](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) la taille des boîtes aux lettres d’archivage en fonction de la licence attribuée au compte d’utilisateur. Lorsque la boîte aux lettres d’archivage atteint 90% de sa taille autorisée, l’utilisateur reçoit une notification par courrier électronique. Lorsqu’une boîte aux lettres d’archivage atteint sa taille limite, l’utilisateur ne peut pas déplacer plus d’éléments vers la boîte aux lettres d’archivage. Office 365 n’augmentera pas la taille d’une boîte aux lettres d’archivage une fois que la limite de taille est atteinte. Au lieu de cela, les utilisateurs peuvent effectuer les actions suivantes pour libérer de l’espace dans la boîte aux lettres d’archivage :

- Exportez les éléments dans un fichier. pst à l’aide d’Outlook.

- Supprimer des éléments de la boîte aux lettres d’archivage.

Office 365 offre un **archivage illimité** pour les licences Office 365 entreprise E3 et E5. Un administrateur doit activer cette fonctionnalité avant que la boîte aux lettres d’archivage atteigne sa taille maximale. Lorsque l’archivage illimité est activé, l’espace disponible peut prendre jusqu’à 30 jours avant d’être ajouté à la boîte aux lettres d’archivage. Par conséquent, nous recommandons aux administrateurs de vérifier l’espace libre dans la boîte aux lettres d’archivage, ce qui permet à l’utilisateur de continuer à utiliser la boîte aux lettres d’archivage pendant qu’elle s’étend. Pour plus d’informations, consultez la rubrique [vue d’ensemble de l’archivage illimité dans office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) et [activation de l’archivage illimité dans Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).

Pour plus d’informations sur l’accès à la boîte aux lettres d’archivage à partir d’Outlook, voir [Configuration requise pour l’accès aux éléments dans un archivage étendu automatiquement](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Pour configurer une stratégie de rétention qui déplace automatiquement les éléments vers la boîte aux lettres d’archivage, consultez [la rubrique Configurer une stratégie d’archivage et de suppression pour les boîtes aux lettres dans votre organisation Office 365](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Remarque**: les archives à extension automatique ne sont pas prises en charge pour les boîtes aux lettres principales sur Exchange 2010.
