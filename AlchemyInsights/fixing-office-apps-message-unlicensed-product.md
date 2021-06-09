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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798678"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="7fc0d-102">L’activation d’Office est impossible</span><span class="sxs-lookup"><span data-stu-id="7fc0d-102">Unable to activate Office</span></span>

<span data-ttu-id="7fc0d-103">**Remarque**: si vous utilisez une version antérieure de Windows (par exemple, Windows 7), vérifiez que TLS 1.2 est activé par défaut.</span><span class="sxs-lookup"><span data-stu-id="7fc0d-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="7fc0d-104">Pour plus d’informations, consultez [Mise à jour pour activer TLS 1.1 et TLS 1.2 comme protocoles sécurisés par défaut dans WinHTTP dans Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="7fc0d-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="7fc0d-105">Vérifiez si votre abonnement a expiré.</span><span class="sxs-lookup"><span data-stu-id="7fc0d-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="7fc0d-106">Assurez-vous que vous disposez d’un abonnement qui autorise les licences client, telles qu’Office 365 Business ou Business Premium, et [s’assurer que l’utilisateur dispose d’une licence attribuée](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="7fc0d-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="7fc0d-107">Assurez-vous que l’utilisateur se connecte à Office avec le compte auquel la licence est attribuée.</span><span class="sxs-lookup"><span data-stu-id="7fc0d-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="7fc0d-108">Consultez la page [état d’intégrité du service Office 365](/office365/enterprise/view-service-health) pour déterminer s’il existe des problèmes connus avec le service.</span><span class="sxs-lookup"><span data-stu-id="7fc0d-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="7fc0d-p102">Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour vérifier qu’ils ne bloquent pas l’accès des applications Microsoft 365 à Internet. Consultez [URL Office 365 et plages d’adresses IP](/office365/enterprise/urls-and-ip-address-ranges "URL et plages d’adresses IP Office 365").</span><span class="sxs-lookup"><span data-stu-id="7fc0d-p102">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet. Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="7fc0d-111">**Conseil** sur les ordinateurs Windows, nous pouvons diagnostiquer et résoudre automatiquement pour vous plusieurs problèmes courants liés à la connexion à Office.</span><span class="sxs-lookup"><span data-stu-id="7fc0d-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="7fc0d-112">Téléchargez et exécutez **[L’Assistant Support et Récupération de Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** pour utiliser notre outil automatisé.</span><span class="sxs-lookup"><span data-stu-id="7fc0d-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="7fc0d-113">Utilisez les informations suivantes relatives à la résolution des problèmes :</span><span class="sxs-lookup"><span data-stu-id="7fc0d-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="7fc0d-114">Ouvrez une application Office, puis [se déconnecter](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de tous les comptes d’utilisateur existants.</span><span class="sxs-lookup"><span data-stu-id="7fc0d-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="7fc0d-115">[Supprimer](/microsoft-365/admin/manage/remove-licenses-from-users) et [réassigner](/microsoft-365/admin/manage/assign-licenses-to-users) la licence Office, puis [Se connecter à Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) à l’aide du compte d’utilisateur assigné.</span><span class="sxs-lookup"><span data-stu-id="7fc0d-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="7fc0d-116">Exécutez l’utilitaire de [Résolution des problèmes d’activation](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="7fc0d-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="7fc0d-117">Réactiver le statut d’activation de Microsoft Office</span><span class="sxs-lookup"><span data-stu-id="7fc0d-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Réactiver le statut d’activation de Microsoft Office")
- [<span data-ttu-id="7fc0d-118">Exécuter une réparation en ligne d’Office</span><span class="sxs-lookup"><span data-stu-id="7fc0d-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="7fc0d-119">Pour d’autres solutions de résolution de problèmes, consultez :</span><span class="sxs-lookup"><span data-stu-id="7fc0d-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="7fc0d-120">Erreurs Produit sans licence et d’activation dans Office</span><span class="sxs-lookup"><span data-stu-id="7fc0d-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="7fc0d-121">Erreur indiquant « Nous sommes désolés, nous ne pouvons pas vous connecter à votre compte. Veuillez essayer de nouveau plus tard » lorsque vous activez Office</span><span class="sxs-lookup"><span data-stu-id="7fc0d-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)