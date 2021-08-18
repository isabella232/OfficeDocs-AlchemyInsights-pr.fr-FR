---
title: Résoudre les problèmes courants liés à la mise en forme des enregistrement DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323988"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Résoudre les problèmes courants liés à la mise en forme des enregistrement DKIM

La plupart des problèmes de mise en place DKIM sont liés à des enregistrements DNS incorrects.

Pour résoudre les problèmes de mise en place de DKIM, vérifiez que l’enregistrement CNAME DKIM **(et** non un enregistrement TXT) est correctement mis en forme. Pour plus d’informations, voir ce que vous devez faire pour [configurer manuellement DKIM dans Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Si vous avez besoin d’aide sur les enregistrements DNS en général, voir Créer des enregistrements DNS auprès d’un fournisseur d’hébergement [DNS pour Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

**Remarque**: après avoir créé ou mis à jour vos enregistrements DNS DKIM sur le service d’hébergement DNS de votre domaine, vous devez attendre que les enregistrements DNS se propagent.
