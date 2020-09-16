---
title: 2491 alerte les messages électroniques provenant de la stratégie « hameçonnage fourni suite à une substitution de client ou d’utilisateur »
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728609"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="a0170-102">Alertez les messages électroniques provenant de la stratégie « hameçonnage fourni suite à une substitution de client ou d’utilisateur »</span><span class="sxs-lookup"><span data-stu-id="a0170-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="a0170-103">Une stratégie d’alerte par défaut nommée « hameçonnage remis en raison de la substitution du client ou de l’utilisateur » a été déployée pour les locataires ayant des licences P1 et P2 Office 365 ATP.</span><span class="sxs-lookup"><span data-stu-id="a0170-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="a0170-104">Si vous avez reçu cette alerte, Voici les étapes à suivre pour examiner :</span><span class="sxs-lookup"><span data-stu-id="a0170-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="a0170-105">Dans le message d’alerte, cliquez sur **afficher l’alerte** pour accéder à la page des **alertes** dans le centre de sécurité & conformité.</span><span class="sxs-lookup"><span data-stu-id="a0170-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="a0170-106">Sélectionnez l’alerte pour voir l’option permettant d' **afficher la liste des messages** ou d’afficher les **messages dans l’Explorateur**.</span><span class="sxs-lookup"><span data-stu-id="a0170-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="a0170-107">Ces deux options vous permettent d’accéder aux détails du message, qui inclut l’ID du message.</span><span class="sxs-lookup"><span data-stu-id="a0170-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="a0170-108">Notez que le lien de l’Explorateur de menaces filtre automatiquement les messages qui correspondent aux critères d’alerte.</span><span class="sxs-lookup"><span data-stu-id="a0170-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="a0170-109">Vous devrez peut-être ajuster le filtre de date dans l’Explorateur de menaces.</span><span class="sxs-lookup"><span data-stu-id="a0170-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="a0170-110">Le message de hameçonnage a été remis en raison d’une substitution configurée manuellement :</span><span class="sxs-lookup"><span data-stu-id="a0170-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="a0170-111">Un expéditeur ou domaine autorisé défini par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a0170-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="a0170-112">Un expéditeur ou domaine autorisé défini par l’administrateur dans une stratégie de blocage du courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="a0170-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="a0170-113">Une adresse IP autorisée dans une stratégie de filtrage des connexions.</span><span class="sxs-lookup"><span data-stu-id="a0170-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="a0170-114">Une règle de flux de messagerie (également appelée règle de transport) qui est configurée pour autoriser les messages dans.</span><span class="sxs-lookup"><span data-stu-id="a0170-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="a0170-115">Si vous pensez que le message a été marqué de manière incorrecte comme hameçonnage, utilisez le [complément de message de rapport](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook pour soumettre des exemples de messages à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a0170-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
