---
title: Relayer le courrier via Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: e971593b7a67e1bb40243fc762bace6b87a35741
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745395"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="4b77a-102">Configurer une application ou un périphérique multi-fonction pour envoyer des courriers électroniques à l’aide d’Office 365</span><span class="sxs-lookup"><span data-stu-id="4b77a-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="4b77a-103">Pour découvrir les options et les étapes, consultez l’article [Comment configurer un appareil ou une application multifonction pour envoyer du courrier électronique à l’aide d’Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="4b77a-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="4b77a-104">**Remarque :** si l’un de vos appareils ou l’une de vos applications a récemment cessé de fonctionner, sachez que nous venons de commencer [la désactivation du chiffrement 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) comme prévu.</span><span class="sxs-lookup"><span data-stu-id="4b77a-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="4b77a-105">Pour afficher les appareils concernés, accédez au [rapport de clients utilisant l’authentification SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="4b77a-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="4b77a-106">Voici quelques erreurs courantes : échec/erreur d’authentification, échec/erreur TLS, erreur d’algorithme de chiffrement, incompatibilité de l’algorithme ou connexion interrompue.</span><span class="sxs-lookup"><span data-stu-id="4b77a-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="4b77a-107">Résolution du problème :</span><span class="sxs-lookup"><span data-stu-id="4b77a-107">To resolve this issue:</span></span>
 - <span data-ttu-id="4b77a-108">**Windows Server 2003 IIS SMTP va cesser de fonctionner : une version plus récente de Windows est nécessaire.**</span><span class="sxs-lookup"><span data-stu-id="4b77a-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="4b77a-109">Contactez votre fournisseur d’application ou d’appareil pour déterminer si un chiffrement moderne est pris en charge ou s’il existe une mise à jour.</span><span class="sxs-lookup"><span data-stu-id="4b77a-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
