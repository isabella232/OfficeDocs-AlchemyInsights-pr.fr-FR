---
title: Utiliser un site web Wix avec des domaines achetés ou gérés par Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: b45923ef112917fb95263dc2690672847129b05f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795053"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a><span data-ttu-id="75da9-102">Utiliser un site web Wix avec des domaines achetés ou gérés par Office 365</span><span class="sxs-lookup"><span data-stu-id="75da9-102">Using Wix website with Office 365 purchased or managed domains</span></span>

- [<span data-ttu-id="75da9-103">Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel</span><span class="sxs-lookup"><span data-stu-id="75da9-103">Update DNS records to keep your website with your current hosting provider</span></span>](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- <span data-ttu-id="75da9-104">L’article de Wix, intitulé « Connecter un domaine à Wix en utilisant la méthode de pointage », recommande d’utiliser la fonction de pointage (ajout d’enregistrements DNS par le lien ci-dessus) plutôt que de modifier les serveurs de noms lorsque vous utilisez Office 365</span><span class="sxs-lookup"><span data-stu-id="75da9-104">Wix article "Connecting a Domain to Wix Using the Pointing Method" recommends using pointing (adding DNS records per the above link) rather than changing names servers when using Office 365</span></span>
- <span data-ttu-id="75da9-105">Si vous choisissez de modifier les serveurs de noms vers WiX, vous devez ensuite  [Créer des enregistrements DNS auprès de WiX pour Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="75da9-105">If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span></span>
- <span data-ttu-id="75da9-106">Si votre domaine a été acheté auprès de Microsoft, les serveurs de noms ne peuvent pas être modifiés.</span><span class="sxs-lookup"><span data-stu-id="75da9-106">If your domain was purchased from Microsoft the name servers cannot be changed.</span></span> <span data-ttu-id="75da9-107">Si vous devez changer de serveur de noms, le domaine acheté par Microsoft doit être  [transféré à un autre fournisseur d’hébergement après 60 jours](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).</span><span class="sxs-lookup"><span data-stu-id="75da9-107">If you have to change names servers the Microsoft purchased domain would need to be  [transferred to another hosting provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span></span>