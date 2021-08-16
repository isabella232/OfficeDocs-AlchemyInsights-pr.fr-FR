---
title: Exemple de stratégie anti-hameçonnage Office 365 Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035004"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Exemple de stratégie anti-hameçonnage Office 365 Microsoft Defender

Ces paramètres activent une stratégie appelée *Domaine et PDG.* Cette stratégie assure la protection des utilisateurs et des domaines contre l’emprunt d’identité, puis applique la stratégie à tous les messages électroniques reçus par les utilisateurs au sein du domaine. Tout d’abord, ajoutez les informations suivantes pour créer la stratégie :

- **Name**: Domain and CEO **Description:** Ensures that the CEO and your domain are not being impersonated.
  **Appliqué à**: Sélectionner **le domaine du destinataire est**. Sous **l’un de ces** éléments, **sélectionnez Choisir,** puis sélectionnez un domaine. Sélectionnez **+ Ajouter**. Cochez la case en regard du nom du domaine dans la liste (par exemple, *contoso.com*), puis sélectionnez **Ajouter**. Sélectionnez **Terminé**.
- Une fois la stratégie créée, vous pouvez affiner la stratégie en utilisant les options suivantes :
  - **Ajoutez des utilisateurs à protéger :** Pour cet exemple, ajoutez au minimum l’adresse e-mail du PDG.
  - **Ajouter des domaines à protéger :** ajoutez le domaine d’organisation qui inclut le bureau du PDG.
  - **Choose actions**: For **If email is sent by an impersonated user,** select Redirect message to another email **address,** and then enter the email address of the security administrator *(for example, securityadmin@contoso.com*). For **If email is sent by an impersonated domain,** select Quarantine the **message**.
  - **Veille sur les** boîtes aux lettres : par défaut, cette option est sélectionnée lorsque vous créez une stratégie anti-hameçonnage. Laissez ce paramètre **activé** pour obtenir de meilleurs résultats.
  - **Ajoutez des expéditeurs et des domaines de confiance :** Pour cet exemple, ne définissez aucune substitution.
- Une fois que vous avez examiné vos paramètres, **sélectionnez Créer cette** stratégie ou **Enregistrer,** le cas échéant.

Pour en savoir plus, consultez [stratégies anti-hameçonnage dans Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
