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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500824"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Résoudre les problèmes courants liés à la mise en forme des enregistrement DKIM

La plupart des problèmes de mise en place DKIM sont liés à des enregistrements DNS incorrects.

Pour résoudre les problèmes de mise en place de DKIM, vérifiez que l’enregistrement CNAME DKIM **(et** non un enregistrement TXT) est correctement mis en forme. Pour plus d’informations, voir ce que vous devez faire pour configurer [manuellement DKIM dans Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Si vous avez besoin d’aide générale sur les enregistrements DNS, voir Créer des enregistrements DNS auprès d’un fournisseur d’hébergement [DNS pour Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Après avoir créé ou mis à jour vos enregistrements DNS DKIM au niveau du service d’hébergement DNS de votre domaine, vous devez attendre que les enregistrements DNS se propagent.
