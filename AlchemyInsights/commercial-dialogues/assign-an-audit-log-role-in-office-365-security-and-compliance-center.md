---
title: Attribuer un rôle Journal d’audit dans le Centre de sécurité et conformité Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 5ddfda8687fe3ae2467ad221c7c083f46239826e23b10b91732ea06fd4649f3e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54006168"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Attribuer un rôle Journal d’audit dans le Centre de sécurité et conformité Office 365

Pour effectuer des recherches dans le journal d’audit Office 365, le rôle **Journaux d’audit en affichage seul** doit être attribué à un administrateur ou au rôle **Journaux d’audit** dans Exchange Online. Par défaut, ces rôles sont affectés aux groupes de rôles Gestion de la conformité et Gestion de l’organisation. Les administrateurs généraux dans votre client Office 365 et Microsoft 365 sont automatiquement des membres du groupe de rôle Gestion de l'organisation.

Pour permettre à un utilisateur d’effectuer des recherches dans le journal d’audit avec le niveau minimal de privilèges, créez un groupe de rôles personnalisé dans Exchange Online, ajouter le rôle **Journaux d’audit en affichage seul** ou **Journaux d’audit**, puis ajouter l’utilisateur en tant que membre du nouveau groupe de rôles.

Pour plus d’informations, consultez [Gérer les groupes de rôles dans Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) et [Effectuer des recherches dans le journal d’audit depuis le Centre de sécurité et conformité ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).