---
title: 'Problèmes de performances : SharePoint ou OneDrive'
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093727"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lent, inaccessible ou indisponible pour plusieurs utilisateurs

Si un site OneDrive ou SharePoint n’est pas disponible pour plusieurs utilisateurs qui y avaient précédemment accès, il peut y avoir un problème de service temporaire. [Vérifiez le tableau de bord d’état du service.](https://portal.office.com/adminportal/home#/servicehealth)

**Ajouter et obtenir une licence pour l’utilisateur**

Assurez-vous [d’attribuer des licences aux utilisateurs Microsoft 365 entreprise.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Attribuer des autorisations**

Si l’utilisateur a reçu une licence SharePoint et reçoit toujours un message de refus d’accès, assurez-vous qu’il dispose du niveau [d’autorisation](https://docs.microsoft.com/sharepoint/understanding-permission-levels) approprié.

**Envisager d’utiliser la fonctionnalité de demande d’accès**

La [fonctionnalité de demande d’accès](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permet aux utilisateurs de demander l’accès au contenu qu’ils n’ont pas l’autorisation de voir actuellement.

**Autoriser un script personnalisé peut entraîner des problèmes d’accès refusé**

Dans certains scénarios, la fonctionnalité autoriser les *scripts* personnalisés peut présenter un accès refusé. Pour obtenir la liste des fonctionnalités concernées, des considérations de sécurité et la possibilité de désactiver la fonctionnalité. Visitez Autoriser [ou empêcher le script personnalisé.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

