---
title: Problèmes de licences Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657274"
---
# <a name="yammer-licensing-issues"></a>Problèmes de licences Yammer

Tous les utilisateurs doivent disposer d’une licence pour pouvoir utiliser le service Yammer Enterprise. Toutefois, par défaut, Yammer n’exige pas que les utilisateurs disposent d’une licence pour accéder au service. Lorsqu’un administrateur modifie le paramètre pour bloquer les utilisateurs de Microsoft 365 sans licence Yammer, les utilisateurs qui ne disposent pas d’une licence Yammer Enterprise ne peuvent pas accéder au service Yammer. Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Gérer les licences utilisateur de Yammer dans Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Lorsque les licences sont retirées aux utilisateurs, la vignette Yammer n’est plus affichée, et les autres services peuvent utiliser la suppression de la licence pour masquer les fonctionnalités. Dans d’autres cas, des fonctionnalités peuvent toujours apparaître, mais nécessitent une attribution de licence pour fonctionner.  

**La licence n’est pas mise à jour pour l’utilisateur**  

Un utilisateur peut parfois se voir attribuer une licence sans toutefois réussir à accéder à Yammer. Les retards sont plus susceptibles de se produire lorsqu’une attribution de licence en masse est en cours. Les utilisateurs de Yammer peuvent ne pas être mis à jour dans le même ordre que les licences sont modifiées dans Azure AD car le système s’exécute de manière asynchrone. Patientez 24 heures avant d’ouvrir un cas de support technique pour signaler les problèmes de synchronisation des licences.  

**Attribution des licences en bloc**  

Les licences peuvent être attribuées via le centre d’administration ou l’écriture de scripts PowerShell. Si vous souhaitez en savoir plus, veuillez consulter les rubriques [Attribuer des licences aux utilisateurs](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) et [Attribuer des licences à des comptes d’utilisateurs avec Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Le support Microsoft ne fournit aucune aide sur la création de scripts, mais la documentation sur l’attribution des licences Yammer est disponible. Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Gérer les licences Yammer à l’aide de Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).