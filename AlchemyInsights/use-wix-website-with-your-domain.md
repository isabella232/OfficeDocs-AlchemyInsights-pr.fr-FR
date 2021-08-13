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
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980175"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Utiliser un site web Wix avec des domaines achetés ou gérés par Office 365

- [Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- L’article de Wix, intitulé « Connecter un domaine à Wix en utilisant la méthode de pointage », recommande d’utiliser la fonction de pointage (ajout d’enregistrements DNS par le lien ci-dessus) plutôt que de modifier les serveurs de noms lorsque vous utilisez Office 365
- Si vous choisissez de modifier les serveurs de noms vers WiX, vous devez ensuite  [Créer des enregistrements DNS auprès de WiX pour Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Si votre domaine a été acheté auprès de Microsoft, les serveurs de noms ne peuvent pas être modifiés. Si vous devez changer de serveur de noms, le domaine acheté par Microsoft doit être  [transféré à un autre fournisseur d’hébergement après 60 jours](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).