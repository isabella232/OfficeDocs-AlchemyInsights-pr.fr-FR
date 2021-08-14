---
title: Erreur d’adresse proxy lors de la création d’une boîte aux lettres partagée
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062906"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Erreur d’adresse proxy lors de la création d’une boîte aux lettres ou d’un autre objet à messagerie

Si vous avez essayé de créer un objet à messagerie (boîte aux lettres, boîte aux lettres partagée, etc.) et que vous avez reçu l’erreur « L’adresse proxy « SMTP:alias@domain.com » est déjà utilisée... », l’adresse de messagerie que vous avez choisie est déjà prise par un autre objet à messagerie dans votre organisation.
  
Vous devez rechercher l’utilisateur, le groupe, la boîte aux lettres partagée ou le dossier public qui possède cette adresse de messagerie et la supprimer ou modifier son adresse de messagerie. Vous pouvez ensuite créer un objet à messagerie avec l’adresse de messagerie libérée. Utilisez la recherche sur la page d’accueil pour la rechercher. Vous pouvez également utiliser la commande PowerShell Exchange Online suivante pour la rechercher :

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Si vous ne souhaitez pas supprimer l’adresse de messagerie existante, choisissez une nouvelle adresse de messagerie pour le nouvel objet que vous créez.
  