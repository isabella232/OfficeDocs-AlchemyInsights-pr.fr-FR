---
title: Résoudre des problèmes de certificat de signature SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: fb043122edf5f99325f0403810eb0dc119d254e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314418"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Résoudre les problèmes de certificat de signature SAML

Pour résoudre un problème de certificat de signature SAML, ces étapes recommandées :

1. Lorsque vous ajoutez une application d’entreprise qui prend en charge l’authentification unique, Azure génère un certificat appelé [Certificat de signature SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Ce certificat a une date d’expiration de 3 ans. Pour modifier la date d’expiration de votre certificat, consultez [Personnaliser la date d’expiration de votre certificat de fédération et en faire un nouveau certificat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure utilisera ce certificat pour signer les jetons SAML demandés par l’application et les envoyer à l’application pour que l’authentification unique s’effectue. Pour ce faire, téléchargez le certificat à partir du portail Azure et envoyez-le au fournisseur de l’application pour finalisation du processus d’authentification unique.

Une fois ce processus terminé, votre application prendra en compte ce certificat et tous les jetons SAML signés par ce certificat seront acceptés par l’application.

3. Si ce certificat arrive à expiration, créez-en un, informez le fournisseur de l’application, puis activez-le sur Azure. Pour plus d’informations, consultez [Renouveler un certificat expirant bientôt](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

**Note**: Si le certificat expire, l’utilisateur ne sera pas bloqué.

4. [Ajoutez une adresse e-mail pour que les notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) soient reçues avant l’expiration du certificat actuel.

**Note**: L’étape 4 est facultative.

5. Modifiez les options de signature du certificat SAML d’une application ainsi que l’algorithme de signature du certificat. Pour plus d’informations, consultez [Modifier des options de signature de certificat et d’un algorithme de signature](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

