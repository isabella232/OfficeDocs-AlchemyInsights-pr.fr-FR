---
title: Problèmes de performances-SharePoint ou OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 9bb18196f38de473e4ee79d77bd43561ad9742e0
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223278"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive est lent, inaccessible ou indisponible pour plusieurs utilisateurs

Si un site OneDrive ou SharePoint n’est pas disponible pour plusieurs utilisateurs qui disposaient précédemment d’un accès, il peut y avoir un problème de service temporaire. [Vérifiez le tableau de bord d’État du service](https://portal.office.com/adminportal/home#/servicehealth).

**Ajouter et accorder une licence à l’utilisateur**

Vérifiez que vous [attribuez des licences aux utilisateurs dans Office 365 pour les entreprises](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


**Attribuer des autorisations**

Si l’utilisateur a reçu une licence SharePoint et qu’il reçoit toujours un message de refus d’accès, vérifiez qu’il dispose du [niveau d’autorisation approprié](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Envisagez d’utiliser la fonctionnalité de demande d’accès**

La [fonctionnalité de demande d’accès](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permet aux utilisateurs de demander l’accès au contenu qu’ils n’ont pas actuellement le droit d’afficher.

**Autoriser le script personnalisé peut entraîner des problèmes de refus d’accès**

Il existe certains scénarios dans lesquels la fonctionnalité *autoriser les scripts personnalisés* peut présenter un accès refusé. Pour obtenir la liste des fonctionnalités affectées, des considérations relatives à la sécurité et la possibilité de désactiver la fonctionnalité. Visitez [ou bloquez le script personnalisé](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

