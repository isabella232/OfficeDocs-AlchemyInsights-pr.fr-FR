---
title: 2491 Alerte des messages électroniques à partir de la stratégie « Hameçonnage remis en raison d’un remplacement par le client ou l’utilisateur »
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544576"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="279df-102">Alerte des messages électroniques à partir de la stratégie « Hameçonnage remis en raison d’un remplacement par le client ou l’utilisateur »</span><span class="sxs-lookup"><span data-stu-id="279df-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="279df-103">Une stratégie d’alerte par défaut nommée « Phish Delivered due to tenant or user override » a été déployée aux clients avec Microsoft Defender pour les licences Office 365 P1 et P2.</span><span class="sxs-lookup"><span data-stu-id="279df-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="279df-104">Si vous avez reçu cette alerte, voici les étapes à suivre pour examiner :</span><span class="sxs-lookup"><span data-stu-id="279df-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="279df-105">Dans le message d’alerte, cliquez sur **Afficher** l’alerte pour aller à la page **Alertes** dans le Centre de sécurité & conformité.</span><span class="sxs-lookup"><span data-stu-id="279df-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="279df-106">Sélectionnez l’alerte pour afficher l’option Afficher la liste **des messages** ou Afficher les messages **dans l’Explorateur.**</span><span class="sxs-lookup"><span data-stu-id="279df-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="279df-107">Ces deux options vous prennent en compte pour obtenir les détails du message, notamment l’ID de message.</span><span class="sxs-lookup"><span data-stu-id="279df-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="279df-108">Notez que le lien Explorateur de menaces filtre automatiquement les messages qui correspondent aux critères d’alerte.</span><span class="sxs-lookup"><span data-stu-id="279df-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="279df-109">Vous devrez peut-être ajuster le filtre de date dans l’Explorateur de menaces.</span><span class="sxs-lookup"><span data-stu-id="279df-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="279df-110">Le message d’hameçonnage a été remis en raison d’une substitution configurée manuellement :</span><span class="sxs-lookup"><span data-stu-id="279df-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="279df-111">Expéditeur ou domaine autorisé par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="279df-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="279df-112">Expéditeur ou domaine autorisé par l’administrateur dans une stratégie anti-courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="279df-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="279df-113">Adresse IP autorisée dans une stratégie de filtrage des connexions.</span><span class="sxs-lookup"><span data-stu-id="279df-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="279df-114">Règle de flux de messagerie (également appelée règle de transport) configurée pour autoriser les messages.</span><span class="sxs-lookup"><span data-stu-id="279df-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="279df-115">Si vous pensez que le message a été marqué à tort comme hameçonnage, utilisez le Outlook signaler un [message](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) pour envoyer des exemples de message à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="279df-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
