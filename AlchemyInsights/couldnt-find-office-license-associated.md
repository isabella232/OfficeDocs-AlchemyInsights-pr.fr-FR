---
title: "Résolution du message : les applications Microsoft 365 n'ont pas pu trouver les licences Office associées"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816486"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Résolution du message « Impossible de trouver les licences Office associées » pour les applications Microsoft 365

Si vous recevez ce message, essayez ce qui suit :

1. Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour vérifier qu'ils ne bloquent pas l'accès Internet aux applications Microsoft 365. Voir [URL et plages d'adresses IP Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Supprimez et [réaffectez la licence Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pour l'utilisateur concerné. 
3. Ouvrez une application Office et [connectez-vous aux](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) comptes d'utilisateurs existants.
4. Go to Windows Settings > **Accounts**  >  **Email & accounts,** and remove all work accounts except the affected account.
5. Accédez à Paramètres Windows > **Comptes** Accès au travail ou à l'école, et déconnectez tous les comptes de travail à l'exception  >  du compte concerné.
6. Réinitialisez l’état d’activation d’Office. [Découvrir comment](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Connectez-vous](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) à l'aide du compte d'utilisateur affecté.

Pour d'autres solutions de dépannage, voir [Les erreurs d'activation](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)et de produit sans licence dans Office.