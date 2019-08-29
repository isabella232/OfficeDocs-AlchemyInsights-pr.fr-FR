---
title: S/MIME dans Outlook sur le Web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666838"
---
# <a name="encrypt-email-messages-in-outlook"></a>Chiffrer les messages électroniques dans Outlook

Le chiffrement de messages Office 365 est basé sur Microsoft Azure Rights Management (Azure RMS), qui fait partie d’Azure information protection. Si votre abonnement inclut Azure Rights Management ou Azure information protection, **il n’est pas nécessaire d’effectuer des actions pour activer ou activer manuellement** le service gestion des droits.

En fonction des commentaires des clients, nous n’allons plus activer les règles de flux de messagerie Exchange pour chiffrer automatiquement les messages électroniques sortants contenant certains types d’informations sensibles dans votre client par défaut. Au lieu de cela, nous fournissons des instructions détaillées pour vous permettre de le faire. Pour plus d’informations sur la création d’une règle de transport pour chiffrer des informations sensibles, consultez [cet article](https://aka.ms/OmeEtr).

- Si vous utilisez Outlook sur le Web (anciennement **owa**): lors de la composition d’un message électronique, cliquez simplement sur **protéger** dans OWA. Cette action s’applique à l’autorisation «ne pas transférer». Cliquez sur **modifier l’autorisation** et sélectionnez **chiffrer** pour uniquement chiffrer le message.

- Si vous utilisez le **client Outlook**: pour envoyer un message chiffré à partir d’Outlook 2013 ou 2016, ou Outlook 2016 pour Mac, sélectionnez **options** > **autorisations**, puis sélectionnez l’option de protection dont vous avez besoin.

- Pour **chiffrer automatiquement tous les messages électroniques** envoyés à certains destinataires ou organisations partenaires externes, vous devez créer une règle de transport de flux de messagerie dans le centre d’administration Exchange. Des instructions détaillées sont fournies dans [cet article de support technique](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

