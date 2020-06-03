---
title: " S/MIME dans Outlook sur le web"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511506"
---
# <a name="encrypt-email-messages-in-outlook"></a>Chiffrer les messages électroniques dans Outlook

Le chiffrement de messages Microsoft 365 est basé sur Microsoft Azure Rights Management (Azure RMS), qui fait partie d’Azure information protection. Si votre abonnement inclut Azure Rights Management ou Azure information protection, **il n’est pas nécessaire d’effectuer des actions pour activer ou activer manuellement** le service gestion des droits.

En fonction des commentaires des clients, nous n’allons plus activer les règles de flux de messagerie Exchange pour chiffrer automatiquement les messages électroniques sortants contenant certains types d’informations sensibles dans votre client par défaut. Au lieu de cela, nous fournissons des instructions détaillées pour vous permettre de le faire. Pour plus d’informations sur la création d’une règle de transport pour chiffrer des informations sensibles, consultez [cet article](https://aka.ms/OmeEtr).

- Si vous utilisez Outlook sur le Web (anciennement **owa**) : lors de la composition d’un message électronique, cliquez simplement sur **protéger** dans OWA. Cette action s’applique à l’autorisation « ne pas transférer ». Cliquez sur **modifier l’autorisation** et sélectionnez **chiffrer** pour uniquement chiffrer le message.

- Si vous utilisez le **client Outlook**: pour envoyer un message chiffré à partir d’Outlook 2013 ou 2016, ou Outlook 2016 pour Mac, sélectionnez **options**  >  **autorisations**, puis sélectionnez l’option de protection dont vous avez besoin.

- Pour **chiffrer automatiquement tous les messages électroniques** envoyés à certains destinataires ou organisations partenaires externes, vous devez créer une règle de transport de flux de messagerie dans le centre d’administration Exchange. Des instructions détaillées sont fournies dans [cet article de support technique](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

