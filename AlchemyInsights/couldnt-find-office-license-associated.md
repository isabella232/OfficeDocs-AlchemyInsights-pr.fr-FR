---
title: Résolution Microsoft 365'applications n’ont pas pu trouver le message associé aux licences Office
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
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069602"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Résolution du message Microsoft 365 applications « Impossible de trouver les licences Office associées »

Si vous recevez ce message, essayez ce qui suit :

1. Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour vérifier qu’ils ne bloquent pas l’accès à Internet Microsoft 365 applications. Voir [Microsoft 365 URL et plages d’adresses IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Supprimez et [réaffectez la licence Office pour](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) l’utilisateur concerné. 
3. Ouvrez un application Office et [connectez-vous aux](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) comptes d’utilisateurs existants.
4. Go to Windows Paramètres > **Accounts**  >  **Email & accounts,** and remove all work accounts except the affected account.
5. Accédez à Windows Paramètres > **compte Access** scolaire ou scolaire et déconnectez tous les comptes de travail à l’exception du compte  >  concerné.
6. Réinitialisez l’état d’activation d’Office. [Découvrir comment](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Connectez-vous](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) à l’aide du compte d’utilisateur affecté.

Pour d’autres solutions de dépannage, voir [Les erreurs d’activation](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)et de produit sans licence dans Office .