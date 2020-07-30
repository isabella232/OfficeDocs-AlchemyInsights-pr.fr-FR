---
title: Profils Wi-Fi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509053"
---
# <a name="intune-wi-fi-profiles"></a>Profils Wi-Fi Intune

La mise en œuvre réussie de la connectivité Wi-Fi pour les clients de gestion des périphériques mobiles dépend d’un profil correctement déployé qui reflète les exigences de l’infrastructure Wi-Fi d’entreprise. Pour examiner les paramètres appropriés pour les plateformes client que vous examinez, voir : 

[Ajouter des paramètres Wi-Fi pour les appareils exécutant Android dans Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Ajouter des paramètres Wi-Fi pour les appareils Android Enterprise dédiés et totalement gérés dans Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[ Ajouter les paramètres du Wi-Fi pour les appareils iOS et iPadOS dans Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Ajouter des paramètres Wi-Fi pour les appareils Windows 10 et versions ultérieures dans Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importer les paramètres Wi-Fi pour les appareils Windows dans Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Problèmes courants**

**Je déploie un profil Wi-Fi dépendant d’un certificat déployé spécifié dans le profil Wi-Fi. Toutefois, les profils de configuration affichent un état d’erreur.**

Vérifiez que votre appareil a reçu le certificat.

1. Dans Intune, accédez à **Tous les appareils** puis sélectionnez l’appareil > **Configuration de l’appareil**.

2. Vérifiez que tous les profils attendus sont répertoriés et que l’état de réussite est vérifié.

3. Pour un profil Android, si vous avez des certificats intermédiaires dans votre chaîne de certificats, assurez-vous qu’ils sont déployés sur les appareils Android.

    Pour vérifier l’état du certificat, accédez à **Configuration des appareils** > **Profils** > **autorité intermédiaire** > **Propriétés** > **Certificat approuvé**.

Si vous continuez à rencontrer des erreurs, passez en revue les sections procédures et résolution des problèmes. Pour plus d’informations, voir [Vue d’ensemble de la résolution des problèmes de profils de certificats SCEP avec Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**J’ai déployé un profil Wi-Fi sur un appareil. Intune indique qu’il a réussi, mais que l’appareil ne se connecte pas au Wi-Fi.**

L’état réussite indique que Intune a correctement déployé le profil configuré. Toutefois, il est possible que ces configurations ne correspondent pas à votre réseau ou d’autres exigences d'authentification. Pour plus d’informations sur la tentative de connexion, passez en revue les journaux dans le service d’infrastructure et d’authentification (sur le contrôleur de point d’accès Wi-Fi et le serveur NPS/RADIUS). Il se peut que vous deviez collaborer avec l’équipe de votre infrastructure réseau ou le fournisseur Wi-Fi tiers pour recueillir et consulter les journaux.