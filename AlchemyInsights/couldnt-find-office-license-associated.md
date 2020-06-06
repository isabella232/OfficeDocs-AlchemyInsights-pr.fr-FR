---
title: Résolution des applications Microsoft 365 les licences Office n’ont pas pu être détectées message associé
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580439"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Résolution du message « Impossible de trouver des licences Office associées » pour Microsoft 365 apps

Si vous recevez ce message, procédez comme suit :

1. Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas l’accès Internet aux applications Microsoft 365. Voir [URL et plages d’adresses IP Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Supprimez et [réaffectez la licence Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pour l’utilisateur concerné. 
3. Ouvrez une application Office et [déconnectez-vous](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de tous les comptes d’utilisateurs existants.
4. Accédez à paramètres **Windows > comptes**de & de  >  **messagerie**et supprimez tous les comptes de travail sauf le compte affecté.
5. Accédez à paramètres Windows > **comptes**  >  **accès professionnel ou scolaire**, puis déconnectez tous les comptes professionnels à l’exception du compte affecté.
6. Réinitialisez l’état d’activation d’Office. [Découvrir comment](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Connectez-vous](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) à l’aide du compte d’utilisateur affecté.

Pour obtenir des solutions de résolution des problèmes supplémentaires, consultez la rubrique [Erreurs d’activation et de produit sans licence dans Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).