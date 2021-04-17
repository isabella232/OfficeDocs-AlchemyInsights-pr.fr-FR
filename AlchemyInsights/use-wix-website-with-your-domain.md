---
title: Utiliser un site web Wix avec des domaines achetés ou gérés par Office 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825945"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Utiliser un site web Wix avec des domaines achetés ou gérés par Office 365

- [Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- L’article de Wix, intitulé « Connecter un domaine à Wix en utilisant la méthode de pointage », recommande d’utiliser la fonction de pointage (ajout d’enregistrements DNS par le lien ci-dessus) plutôt que de modifier les serveurs de noms lorsque vous utilisez Office 365
- Si vous choisissez de modifier les serveurs de noms vers WiX, vous devez ensuite  [Créer des enregistrements DNS auprès de WiX pour Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Si votre domaine a été acheté auprès de Microsoft, les serveurs de noms ne peuvent pas être modifiés. Si vous devez changer de serveur de noms, le domaine acheté par Microsoft doit être  [transféré à un autre fournisseur d’hébergement après 60 jours](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).