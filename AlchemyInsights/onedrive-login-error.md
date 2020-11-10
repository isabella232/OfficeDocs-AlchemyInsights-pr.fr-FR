---
title: Erreur de connexion OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947486"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="a1691-102">Erreur de connexion OneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="a1691-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="a1691-103">Si vous recevez une erreur « AADSTS50011 : l’URL de réponse spécifiée dans la demande ne correspond pas à la réponse » lorsque vous vous connectez à l’application OneDrive, vérifiez les points suivants :</span><span class="sxs-lookup"><span data-stu-id="a1691-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="a1691-104">Votre version de OneDrive doit être supérieure ou égale à la version 20.052. XXXX. XX.</span><span class="sxs-lookup"><span data-stu-id="a1691-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="a1691-105">Pour vérifier votre version, cliquez sur l’icône OneDrive en bleu dans la zone de notification, sélectionnez **aide & paramètres > paramètres > à propos** de.</span><span class="sxs-lookup"><span data-stu-id="a1691-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="a1691-106">Votre réseau peut bloquer le trafic vers **g.live.com** et **oneclient.SFX.ms**.</span><span class="sxs-lookup"><span data-stu-id="a1691-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="a1691-107">Si ce trafic est bloqué, OneDrive ne peut pas se mettre à jour lui-même.</span><span class="sxs-lookup"><span data-stu-id="a1691-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="a1691-108">Collaborez avec votre administrateur réseau pour vous assurer que vous avez accès à ces URL.</span><span class="sxs-lookup"><span data-stu-id="a1691-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="a1691-109">[Ces points de terminaison](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) doivent être accessibles aux clients qui utilisent des plans Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a1691-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="a1691-110">Si vous avez besoin d’obtenir manuellement une version actuelle de OneDrive, visitez [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="a1691-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
