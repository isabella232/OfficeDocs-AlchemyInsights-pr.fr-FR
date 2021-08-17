---
title: Les stratégies de rétention Exchange centre d’administration ne fonctionnent pas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074930"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Stratégies de rétention dans Exchange Admin Center

Si vous souhaitez que nous 2007-2016 exécutez des vérifications automatisées pour les paramètres mentionnés ci-dessous, sélectionnez le bouton Retour <- en haut de cette page, puis entrez l’adresse e-mail de l’utilisateur qui a des problèmes avec les stratégies de rétention.

Si vous avez des problèmes avec les stratégies de rétention dans le Centre d’administration Exchange ne s’appliquant pas aux boîtes aux lettres ou aux éléments qui ne sont pas en déplacement vers la boîte aux lettres d’archivage, vérifiez les points suivants :

**Causes premières :**

- **L’Assistant Dossier géré** n’a pas traitée la boîte aux lettres de l’utilisateur. L’Assistant Dossier géré tente de traiter toutes les boîtes aux lettres de votre organisation en nuage tous les sept jours.

  **Solution :** Exécutez l’Assistant Dossier géré.

- **RetentionHold** a été **activé sur la** boîte aux lettres. Si la boîte aux lettres a été placée sur un retentionHold, la stratégie de rétention sur la boîte aux lettres ne sera pas traitée pendant cette période.

  **Solution :** Vérifiez l’état du paramètre conservation de rétention et mettez-le à jour selon vos besoins. Pour plus d’informations, voir [Conservation de rétention de boîte aux lettres.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Remarque :** Si une boîte aux lettres est plus petite que 10 Mo, l’Assistant Dossier géré ne traitera pas automatiquement la boîte aux lettres.
 
Pour plus d’informations sur les stratégies de rétention dans Exchange Admin Center, voir :

- [Balises et stratégies de rétention](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Appliquer une stratégie de rétention à des boîtes aux lettres](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ou ajouter ou supprimer des [balises de rétention](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Comment identifier le type de conservation placé sur une boîte aux lettres](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
