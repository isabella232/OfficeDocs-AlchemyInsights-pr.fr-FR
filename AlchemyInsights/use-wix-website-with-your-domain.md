---
title: Utiliser un site web Wix avec des domaines achetés ou gérés par Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300702"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Utiliser un site web Wix avec des domaines achetés ou gérés par Office 365

- [Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- L’article de Wix, intitulé « Connecter un domaine à Wix en utilisant la méthode de pointage », recommande d’utiliser la fonction de pointage (ajout d’enregistrements DNS par le lien ci-dessus) plutôt que de modifier les serveurs de noms lorsque vous utilisez Office 365
- Si vous choisissez de modifier les serveurs de noms vers WiX, vous devez ensuite  [Créer des enregistrements DNS auprès de WiX pour Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Si votre domaine a été acheté auprès de Microsoft, les serveurs de noms ne peuvent pas être modifiés. Si vous devez changer de serveur de noms, le domaine acheté par Microsoft doit être  [transféré à un autre fournisseur d’hébergement après 60 jours](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).