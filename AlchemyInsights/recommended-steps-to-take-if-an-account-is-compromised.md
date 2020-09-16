---
title: Mesures recommandées si un compte est compromis
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: acce676ebb9f4000794669ffb268e7b4fe057f77
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771278"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a>Mesures recommandées si un compte est compromis

[VIDÉO : Réparation d’un compte compromis](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. [Réinitialisez immédiatement le mot de passe de l’utilisateur](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords). Ne transmettez pas le nouveau mot de passe par courrier électronique à l’utilisateur final.

2. Supprimez les [adresses de transfert](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding) suspectes définies au niveau de la boîte aux lettres.

3. Supprimez les [règles de boîte de réception](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) suspectes définies dans la boîte aux lettres.

4. Si l’utilisateur ne peut pas envoyer d’e-mail, [accédez à la page Utilisateurs restreints pour débloquer le compte](https://protection.office.com/?hash=/restrictedusers). Une fois cette opération effectuée, l’utilisateur doit pouvoir reprendre l’envoi de messages dans l’heure qui suit.

5. Supprimez le compte d’utilisateur de tout [groupe doté d’un rôle administratif](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles) jusqu’à ce que vous soyez certain qu’il n’est plus compromis.

Pour minimiser le risque de violation de données ou de compromission du compte à l’avenir, nous vous recommandons de lire notre [feuille de route de sécurité Microsoft 365](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).
  