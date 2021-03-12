---
title: Configurer DKIM avec des domaines personnalisés
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735796"
---
# <a name="set-up-dkim-with-custom-domains"></a>Configurer DKIM avec des domaines personnalisés

Vous devez publier deux enregistrements CNAME pour chaque domaine personnalisé dans DNS. Pour ce faire, utilisez le format suivant :

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** est le texte à gauche de **.mail.protection.outlook.com** dans l’enregistrement MX personnalisé pour le domaine personnalisé (par exemple, contoso-com pour le domaine **contoso.com**). **InitialDomain est** le domaine que vous avez utilisé lorsque vous vous êtes inscrit à Office 365 (par **exemple, contoso.onmicrosoft.com**).

Pour plus d’informations sur les enregistrements DNS, voir Créer des enregistrements DNS chez un fournisseur d’hébergement [DNS pour Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)