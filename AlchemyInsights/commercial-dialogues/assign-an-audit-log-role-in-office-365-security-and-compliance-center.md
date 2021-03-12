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
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736851"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="5c5c3-102">Attribuer un rôle Journal d’audit dans le Centre de sécurité et conformité Office 365</span><span class="sxs-lookup"><span data-stu-id="5c5c3-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="5c5c3-103">Pour effectuer des recherches dans le journal d’audit Office 365, le rôle **Journaux d’audit en affichage seul** doit être attribué à un administrateur ou au rôle **Journaux d’audit** dans Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5c5c3-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="5c5c3-104">Par défaut, ces rôles sont affectés aux groupes de rôles Gestion de la conformité et Gestion de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="5c5c3-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="5c5c3-105">Les administrateurs généraux dans votre client Office 365 et Microsoft 365 sont automatiquement des membres du groupe de rôle Gestion de l'organisation.</span><span class="sxs-lookup"><span data-stu-id="5c5c3-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="5c5c3-106">Pour permettre à un utilisateur d’effectuer des recherches dans le journal d’audit avec le niveau minimal de privilèges, créez un groupe de rôles personnalisé dans Exchange Online, ajouter le rôle **Journaux d’audit en affichage seul** ou **Journaux d’audit**, puis ajouter l’utilisateur en tant que membre du nouveau groupe de rôles.</span><span class="sxs-lookup"><span data-stu-id="5c5c3-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="5c5c3-107">Pour plus d’informations, consultez [Gérer les groupes de rôles dans Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) et [Effectuer des recherches dans le journal d’audit depuis le Centre de sécurité et conformité ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="5c5c3-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>