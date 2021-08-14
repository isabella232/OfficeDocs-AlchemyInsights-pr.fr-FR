---
title: Résoudre les problèmes courants liés à la mise en forme d’enregistrement DKIM
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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930059"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Résoudre les problèmes courants liés à la mise en forme d’enregistrement DKIM

La plupart des problèmes de mise en place DKIM sont liés à des enregistrements DNS incorrects.

Pour résoudre les problèmes de mise en place de DKIM, vérifiez que l’enregistrement CNAME DKIM **(et** non un enregistrement TXT) est correctement mis en forme. Pour plus d’informations, voir ce que vous devez faire pour [configurer manuellement DKIM dans Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Si vous avez besoin d’aide sur les enregistrements DNS en général, voir Créer des enregistrements DNS auprès d’un fournisseur d’hébergement [DNS pour Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Après avoir créé ou mis à jour vos enregistrements DNS DKIM sur le service d’hébergement DNS de votre domaine, vous devez attendre que les enregistrements DNS se propagent.
