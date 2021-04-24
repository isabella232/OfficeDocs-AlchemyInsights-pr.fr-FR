---
title: Les stratégies de rétention dans le Centre d'administration Exchange ne fonctionnent pas
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952226"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Stratégies de rétention dans le Centre d'administration Exchange

Si vous souhaitez que nous 2007-2016 exécutez des vérifications automatisées pour les paramètres mentionnés ci-dessous, sélectionnez le bouton Retour <- en haut de cette page, puis entrez l'adresse e-mail de l'utilisateur qui a des problèmes avec les stratégies de rétention.

Si vous avez des problèmes avec les stratégies de rétention dans le Centre d'administration Exchange qui ne s'appliquent pas aux boîtes aux lettres ou aux éléments qui ne sont pas en déplacement vers la boîte aux lettres d'archivage, vérifiez les points suivants :

**Causes premières :**

- **L'Assistant Dossier géré** n'a pas traitée la boîte aux lettres de l'utilisateur. L'Assistant Dossier géré tente de traiter toutes les boîtes aux lettres de votre organisation en nuage tous les sept jours.

  **Solution :** Exécutez l'Assistant Dossier géré.

- **RetentionHold** a été **activé sur la** boîte aux lettres. Si la boîte aux lettres a été placée sur un retentionHold, la stratégie de rétention sur la boîte aux lettres n'est pas traitée pendant cette période.

  **Solution :** Vérifiez l'état du paramètre conservation de rétention et mettez-le à jour selon vos besoins. Pour plus d'informations, voir [Conservation de rétention de boîte aux lettres.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Remarque :** Si une boîte aux lettres est plus petite que 10 Mo, l'Assistant Dossier géré ne traitera pas automatiquement la boîte aux lettres.
 
Pour plus d'informations sur les stratégies de rétention dans le Centre d'administration Exchange, voir :

- [Balises et stratégies de rétention](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Appliquer une stratégie de rétention à des boîtes aux lettres](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ou ajouter ou supprimer des [balises de rétention](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Comment identifier le type de conservation placé sur une boîte aux lettres](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
