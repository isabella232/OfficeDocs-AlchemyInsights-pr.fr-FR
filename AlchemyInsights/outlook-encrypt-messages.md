---
title: " S/MIME dans Outlook sur le web"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010722"
---
# <a name="encrypt-email-messages-in-outlook"></a>Chiffrer les messages électroniques dans Outlook

Microsoft 365 Le chiffrement des messages est Microsoft Azure Rights Management (Azure RMS), qui fait partie d’Azure Information Protection. Si votre abonnement inclut Azure Rights Management ou Azure Information Protection, vous n’avez pas besoin de prendre des **mesures** pour activer ou activer manuellement le service Rights Management.

En fonction des commentaires des clients, nous n’activerons plus les règles de flux de messagerie Exchange pour chiffrer automatiquement les messages sortants contenant certains types d’informations sensibles dans votre client par défaut. Au lieu de cela, nous fournissons des instructions détaillées sur la façon dont vous pouvez le faire. Pour plus d’informations sur la création d’une règle de transport pour chiffrer des informations sensibles, consultez [cet article.](https://aka.ms/OmeEtr)

- Si vous utilisez Outlook sur le Web (anciennement **OWA)**: lors  de la composition d’un message électronique, cliquez simplement sur Protéger dans OWA. Cela s’applique à l’autorisation « Ne pas avancer ». Cliquez **sur Modifier l’autorisation** et **choisissez Chiffrer** pour chiffrer uniquement le message.

- Si vous utilisez **Outlook client**: pour envoyer un message chiffré à partir de Outlook 2013 ou 2016 ou Outlook 2016 pour Mac, sélectionnez **Options**  >  **Permissions,** puis sélectionnez l’option de protection dont vous avez besoin.

- Pour **chiffrer automatiquement** tous les messages envoyés à certains destinataires ou organisations partenaires externes, vous devez créer une règle de transport de flux de messagerie dans le Centre d Exchange’administration. Des instructions détaillées sont fournies dans [cet article de support.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

