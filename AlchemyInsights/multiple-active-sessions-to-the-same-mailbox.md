---
title: Plusieurs sessions actives dans la même boîte aux lettres
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769721"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="49adb-102">Plusieurs sessions actives dans la même boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="49adb-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="49adb-103">Pour contrôler l’utilisation des ressources Exchange, une boîte aux lettres dispose d’un « budget ».</span><span class="sxs-lookup"><span data-stu-id="49adb-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="49adb-104">L’exception de dépassement budgétaire peut être déclenchée par, mais n’est pas limitée aux conditions suivantes :</span><span class="sxs-lookup"><span data-stu-id="49adb-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="49adb-105">Certains onglets de navigateur sont ouverts dans la même session Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="49adb-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="49adb-106">Quelques sessions Outlook Web App sont actives dans la même boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="49adb-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="49adb-107">D’autres applications clientes (Outlook, Outlook Mobile, application client tierce) accèdent à la boîte aux lettres en même temps.</span><span class="sxs-lookup"><span data-stu-id="49adb-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="49adb-108">Les opérations de longue durée, telles que l’exécution de requêtes de recherche, sont effectuées à partir d’une autre session active de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="49adb-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

