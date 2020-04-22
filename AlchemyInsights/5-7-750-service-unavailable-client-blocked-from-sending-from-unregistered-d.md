---
title: 1048 5.7.750 service non disponible. Le client a bloqué l’envoi à partir de domaines non enregistrés
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676711"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="c4b18-103">Client 5.7.750 interdit d’envoi à partir d’un domaine non enregistré</span><span class="sxs-lookup"><span data-stu-id="c4b18-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="c4b18-104">L’erreur se produit lorsqu’un grand nombre de messages sont envoyés à partir de domaines qui ne sont pas configurés dans votre client (ajoutés en tant que domaines acceptés et validés).</span><span class="sxs-lookup"><span data-stu-id="c4b18-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="c4b18-105">Pour éviter cette erreur, vous pouvez utiliser un connecteur de flux de messagerie basé sur un certificat où le domaine du certificat est un domaine configuré, ou vous pouvez configurer tous les domaines d’envoi.</span><span class="sxs-lookup"><span data-stu-id="c4b18-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
