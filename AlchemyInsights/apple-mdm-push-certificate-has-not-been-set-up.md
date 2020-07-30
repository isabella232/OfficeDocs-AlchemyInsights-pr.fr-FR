---
title: Le certificat Push Apple GPM n’a pas été configuré
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431461"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Le certificat Push Apple GPM n’a pas été configuré

Un certificat Push Apple GPM (également appelé certificat Push Apple Notification Service (APNS)) n’a pas été configuré pour votre abonnement. Si vous n’avez pas configuré un certificat Apple GPM push, vous ne pouvez pas inscrire et gérer les appareils iOS et MacOS. Après avoir ajouté le certificat à Intune, les utilisateurs peuvent installer l'application Company Portal pour enregistrer leurs appareils iOS.

1. Sélectionnez **« J’accepte ».** pour accorder à Microsoft l’autorisation d’envoyer des données à Apple.

2. Sélectionnez **Télécharger votre conseiller du service clientèle** la demande de signature de certificat Intune requise pour créer un certificat Apple GPM pour Push. Le fichier est utilisé pour demander un certificat de relation de confiance à partir du Portail de certificats Push Apple.

3. Sélectionnez **Créer votre certificat Push GPM** pour accéder au Portail certificats Push Apple. Connectez-vous avec l'identifiant Apple de votre entreprise, puis sélectionnez **Créer un certificat**. Sélectionnez **Choisir fichier**, accédez au fichier de demande de signature de certificat, puis sélectionnez **Télécharger**. Sur la page de confirmation, sélectionnez **Télécharger** pour télécharger le fichier (.pem) du certificat et enregistrer le fichier en local.
 
**Remarque**: le certificat est associé à l’ID Apple utilisé pour le créer. Nous vous conseillons d’utiliser un ID Apple d’entreprise pour les tâches de gestion et de vérifier que la boîte aux lettres est contrôlée par plusieurs personnes ou à l’aide d’une liste de distribution. N'utilisez jamais un identifiant Apple personnel. Utilisez le même ID Apple pour renouveler le certificat Push Apple tous les 12 mois.
 
4. Entrez l'ID Apple utilisé pour créer votre certificat de push GPM Apple. Enregistrez cet ID comme rappel pour lorsque vous avez besoin de renouveler le certificat.

5. Accédez au fichier de certificat (.pem), sélectionnez **Ouvrir**, puis sélectionnez **Télécharger**. Avec le certificat push, Intune peut inscrire et gérer les appareils Apple.