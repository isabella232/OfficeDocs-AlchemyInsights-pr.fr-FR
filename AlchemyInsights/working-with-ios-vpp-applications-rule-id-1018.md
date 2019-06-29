---
title: Utilisation de l’ID de règle des applications VPP iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364848"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="5909e-102">Utilisation des applications VPP iOS</span><span class="sxs-lookup"><span data-stu-id="5909e-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="5909e-103">Découvrez [Comment gérer les applications iOS achetées via un programme d’achat en volume avec Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) pour en savoir plus sur les fonctionnalités, les contraintes et les étapes à suivre pour utiliser le programme d’achat en volume Apple et la prise en charge de celui-ci dans Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="5909e-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="5909e-104">**Problèmes courants:** «J’ai affecté une application iOS VPP à mes utilisateurs, mais l’installation a échoué».</span><span class="sxs-lookup"><span data-stu-id="5909e-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="5909e-105">Cela peut se produire si un seul jeton VPP est utilisé sur plusieurs fournisseurs de gestion des appareils mobiles.</span><span class="sxs-lookup"><span data-stu-id="5909e-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="5909e-106">Les jetons VPP d’Apple ne peuvent être utilisés qu’avec un seul fournisseur.</span><span class="sxs-lookup"><span data-stu-id="5909e-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="5909e-107">Si vous avez utilisé un jeton VPP avec plusieurs fournisseurs, vous devez télécharger de nouveau le jeton vers Intune.</span><span class="sxs-lookup"><span data-stu-id="5909e-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="5909e-108">L’installation peut également échouer si le nombre total d’installations est supérieur au nombre de licences.</span><span class="sxs-lookup"><span data-stu-id="5909e-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="5909e-109">Pour afficher un rapport d’utilisation pour vos licences, accédez à la page des \> **licences d’application** pour les **applications mobiles Intune** .</span><span class="sxs-lookup"><span data-stu-id="5909e-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="5909e-110">Pour savoir comment récupérer des licences en cours d’utilisation, reportez-vous à [cet article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="5909e-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
