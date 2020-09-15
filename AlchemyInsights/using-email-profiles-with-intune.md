---
title: Utilisation de profils de messagerie avec Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653286"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="9285f-102">Utilisation de profils de messagerie avec Intune</span><span class="sxs-lookup"><span data-stu-id="9285f-102">Using email profiles with Intune</span></span>

<span data-ttu-id="9285f-103">Intune peut être utilisé pour créer et déployer des profils de messagerie pour le client de courrier natif (intégré) sur plusieurs plateformes d’appareils.</span><span class="sxs-lookup"><span data-stu-id="9285f-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="9285f-104">Pour plus d’informations sur les restrictions associées aux profils de messagerie, notamment sur le traitement de la présence de profils existants et la suppression de profils de messagerie, consultez [Ajouter des paramètres de courrier aux appareils à l’aide de Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="9285f-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="9285f-105">Pour plus d’informations sur la création de profils de messagerie pour chaque plateforme d’appareil, consultez :</span><span class="sxs-lookup"><span data-stu-id="9285f-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="9285f-106">Paramètres de l’appareil Android pour configurer le courrier, l’authentification et la synchronisation dans Intune</span><span class="sxs-lookup"><span data-stu-id="9285f-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="9285f-107"> Ajouter les paramètres de courrier électronique pour les appareils iOS et iPadOS dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9285f-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="9285f-108">Paramètres de profil de messagerie dans Microsoft Intune pour les appareils exécutant Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="9285f-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="9285f-109">Paramètres de profil de messagerie pour les appareils exécutant Windows 10 dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9285f-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="9285f-110">**Problème de synchronisation courants**</span><span class="sxs-lookup"><span data-stu-id="9285f-110">**Common syncing issue**</span></span>

<span data-ttu-id="9285f-111">**L’utilisation d’un profil de messagerie KNOX sur Android empêche les contacts, le calendrier et les tâches de se synchroniser avec les appareils utilisateur.**</span><span class="sxs-lookup"><span data-stu-id="9285f-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="9285f-112">Le profil de courriel KNOX sur Android KNOX offre à l'administrateur la possibilité de décider quels types de contenu sont synchronisés avec l'appareil en définissant chacun sur activé.</span><span class="sxs-lookup"><span data-stu-id="9285f-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="9285f-113">Si le paramètre de n’importe quel type de contenu est défini sur **Non configuré** (valeur par défaut), ce type de contenu n’est pas synchronisé automatiquement.</span><span class="sxs-lookup"><span data-stu-id="9285f-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="9285f-114">Un utilisateur peut activer le type de contenu qu’il souhaite utiliser directement sur l’appareil manuellement, mais cette configuration est remplacée par le paramètre de stratégie Intune, et la synchronisation s’arrête pour ce type de contenu.</span><span class="sxs-lookup"><span data-stu-id="9285f-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

