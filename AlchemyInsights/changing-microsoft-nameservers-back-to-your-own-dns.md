---
title: Modification des serveurs de noms Microsoft pour revenir à la gestion de vos propres enregistrements DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481848"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Modification des serveurs de noms Microsoft pour revenir à la gestion de vos propres enregistrements DNS

Vous avez précédemment modifié vos enregistrements NS pour qu’ils pointent vers Microsoft (ns1.bdm.microsoftonline.com), mais vous avez décidé de gérer vos propres enregistrements DNS :

Sur le site web de votre bureau d’enregistrement de domaines, revenez au nom de votre bureau d’enregistrement ou à votre paramètre précédent. Si vous n'êtes pas familiarisé avec DNS, contactez le support du bureau d'enregistrement de domaines. Notez que les modifications de serveur de noms peuvent prendre jusqu'à 48 heures. 

1. Dans le portail Administration Microsoft 365, accédez à **Paramètres** > [**Domaines**](https://admin.microsoft.com/Adminportal/Home#/Domains), cochez la case en regard du domaine, puis sélectionnez **Gérer DNS**. 

2. Dans l’Assistant, sélectionnez **Ajouter vos propres enregistrements DNS**, puis terminez l’Assistant. Cela modifie la façon dont votre DNS est géré et vous permet ensuite d’ajouter les enregistrements DNS personnalisés nécessaires pour prendre en charge vos services sélectionnés.

Si vous avez changé vos enregistrements de serveur de noms en Microsoft et que vous avez un site web, vous pouvez également ajouter des enregistrements DNS pour le site web au lieu de modifier les serveurs de noms. Pour plus d’informations, voir [Mettre à jour les enregistrements DNS pour conserver votre site web auprès de votre fournisseur d’hébergement actuel](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).


