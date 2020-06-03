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
ms.openlocfilehash: f80b2a10ebc17cd98ed1d29b0e6ba3ca01eb1d62
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508806"
---
# <a name="increase-the-archive-mailbox-size"></a>Augmenter la taille de la boîte aux lettres d’archivage

Microsoft 365 [limite](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) la taille des boîtes aux lettres d’archivage en fonction de la licence attribuée au compte d’utilisateur. Lorsque la boîte aux lettres d’archivage atteint 90% de sa taille autorisée, l’utilisateur reçoit une notification par courrier électronique. Lorsqu’une boîte aux lettres d’archivage atteint sa taille limite, l’utilisateur ne peut pas déplacer plus d’éléments vers la boîte aux lettres d’archivage. Microsoft 365 n’augmentera pas la taille d’une boîte aux lettres d’archivage une fois la limite de taille atteinte. Au lieu de cela, les utilisateurs peuvent effectuer les actions suivantes pour libérer de l’espace dans la boîte aux lettres d’archivage :

- Exportez les éléments dans un fichier. pst à l’aide d’Outlook.

- Supprimer des éléments de la boîte aux lettres d’archivage.

Microsoft 365 fournit un **archivage illimité** pour les licences Office 365 entreprise E3 et E5. Un administrateur doit activer cette fonctionnalité avant que la boîte aux lettres d’archivage atteigne sa taille maximale. Lorsque l’archivage illimité est activé, l’espace disponible peut prendre jusqu’à 30 jours avant d’être ajouté à la boîte aux lettres d’archivage. Par conséquent, nous recommandons aux administrateurs de vérifier l’espace libre dans la boîte aux lettres d’archivage, ce qui permet à l’utilisateur de continuer à utiliser la boîte aux lettres d’archivage pendant qu’elle s’étend. Pour plus d’informations, reportez-vous à la rubrique [Overview of Unlimited Archiving in microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) et [Enable Unlimited Archiving dans Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Pour plus d’informations sur l’accès à la boîte aux lettres d’archivage à partir d’Outlook, voir [Configuration requise pour l’accès aux éléments dans un archivage étendu automatiquement](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Pour configurer une stratégie de rétention qui déplace automatiquement les éléments vers la boîte aux lettres d’archivage, consultez la rubrique [configurer une stratégie d’archivage et de suppression pour les boîtes aux lettres dans votre organisation Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Remarque**: les archives à extension automatique ne sont pas prises en charge pour les boîtes aux lettres principales sur Exchange 2010.
