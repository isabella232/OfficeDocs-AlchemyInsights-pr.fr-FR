---
title: L’activation d’Office est impossible
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928367"
---
# <a name="unable-to-activate-office"></a>L’activation d’Office est impossible

**Remarque**: si vous utilisez une version antérieure de Windows (par exemple, Windows 7), vérifiez que TLS 1.2 est activé par défaut. Pour plus d’informations, consultez [Mise à jour pour activer TLS 1.1 et TLS 1.2 comme protocoles sécurisés par défaut dans WinHTTP dans Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

- Vérifiez si votre abonnement a expiré.
- Assurez-vous que vous disposez d’un abonnement qui autorise les licences client, telles qu’Office 365 Business ou Business Premium, et [s’assurer que l’utilisateur dispose d’une licence attribuée](/microsoft-365/admin/manage/assign-licenses-to-users).
- Assurez-vous que l’utilisateur se connecte à Office avec le compte auquel la licence est attribuée.
- Consultez la page [état d’intégrité du service Office 365](/office365/enterprise/view-service-health) pour déterminer s’il existe des problèmes connus avec le service.
- Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour vérifier qu’ils ne bloquent pas l’accès des applications Microsoft 365 à Internet. Consultez [URL Office 365 et plages d’adresses IP](/office365/enterprise/urls-and-ip-address-ranges "URL et plages d’adresses IP Office 365").

**Conseil** sur les ordinateurs Windows, nous pouvons diagnostiquer et résoudre automatiquement pour vous plusieurs problèmes courants liés à la connexion à Office. Téléchargez et exécutez **[L’Assistant Support et Récupération de Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** pour utiliser notre outil automatisé.

Utilisez les informations suivantes relatives à la résolution des problèmes :

- Ouvrez une application Office, puis [se déconnecter](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de tous les comptes d’utilisateur existants. [Supprimer](/microsoft-365/admin/manage/remove-licenses-from-users) et [réassigner](/microsoft-365/admin/manage/assign-licenses-to-users) la licence Office, puis [Se connecter à Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) à l’aide du compte d’utilisateur assigné.
- Exécutez l’utilitaire de [Résolution des problèmes d’activation](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Réactiver le statut d’activation de Microsoft Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Réactiver le statut d’activation de Microsoft Office")
- [Exécuter une réparation en ligne d’Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Pour d’autres solutions de résolution de problèmes, consultez :  

- [Erreurs Produit sans licence et d’activation dans Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Erreur indiquant « Nous sommes désolés, nous ne pouvons pas vous connecter à votre compte. Veuillez essayer de nouveau plus tard » lorsque vous activez Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)