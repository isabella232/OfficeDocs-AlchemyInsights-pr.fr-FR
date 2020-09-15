---
title: Interruption des mises à jour planifiées
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721553"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="10111-102">Interruption des mises à jour planifiées</span><span class="sxs-lookup"><span data-stu-id="10111-102">Pausing scheduled updates</span></span>

<span data-ttu-id="10111-103">Lorsqu’une commande d’interruption est émise, les appareils ne traitent la commande que la prochaine fois qu’ils archivent dans Intune.</span><span class="sxs-lookup"><span data-stu-id="10111-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="10111-104">Pour cette raison, vos appareils peuvent avoir :</span><span class="sxs-lookup"><span data-stu-id="10111-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="10111-105">Installé les mises à jour planifiées avant l’archivage.</span><span class="sxs-lookup"><span data-stu-id="10111-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="10111-106">Été hors tension lorsque vous avez émis la commande d’interruption.</span><span class="sxs-lookup"><span data-stu-id="10111-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="10111-107">Dans ce cas, lorsque les appareils sont sous tension, ils ont peut-être téléchargé et installé les mises à jour planifiées avant l’archivage.</span><span class="sxs-lookup"><span data-stu-id="10111-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>