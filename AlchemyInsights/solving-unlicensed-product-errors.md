---
title: Résolution des erreurs de produit sans licence
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737951"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Suggestions de résolution des erreurs « produit sans licence »

Pour résoudre les erreurs relatives à un produit « sans licence », procédez comme suit :

- Vérifiez si l’état de votre abonnement a expiré.
- Assurez-vous que vous disposez d’un abonnement qui autorise les licences client, telles que Microsoft 365 apps pour les entreprises ou Business Premium, et [Assurez-vous qu’une licence a été attribuée à l’utilisateur](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Assurez-vous que l’utilisateur se connecte à Office avec le même compte auquel la licence est attribuée.
- Consultez la [page État du service](https://docs.microsoft.com/office365/enterprise/view-service-health) pour voir s’il existe des problèmes connus avec le service.
- Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas les applications Microsoft 365 Access sur Internet. Voir [URL et plages d’adresses IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Vous pouvez également essayer les actions de dépannage suivantes : 

- Ouvrez une application Office et [déconnectez-vous](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de tous les comptes d’utilisateurs existants. [Supprimez](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) et [réaffectez](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) la licence Office, puis [Connectez-vous à Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) à l’aide du compte d’utilisateur affecté.
- Exécutez l' [utilitaire de résolution des problèmes d’activation](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Réinitialisez l’état d’activation d’Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Effectuer une réparation en ligne d’Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Pour d’autres solutions de résolution de problèmes, consultez : 

- [Erreurs Produit sans licence et d’activation dans Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Erreur indiquant « Nous sommes désolés, nous ne pouvons pas vous connecter à votre compte. Veuillez essayer de nouveau plus tard » lorsque vous activez Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)