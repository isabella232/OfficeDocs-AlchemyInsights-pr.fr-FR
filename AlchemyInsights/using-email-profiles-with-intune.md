---
title: Utilisation de profils de messagerie avec Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505192"
---
# <a name="using-email-profiles-with-intune"></a>Utilisation de profils de messagerie avec Intune

Intune peut être utilisé pour créer et déployer des profils de messagerie pour le client de courrier natif (intégré) sur plusieurs plateformes d’appareils.

Pour plus d’informations sur les restrictions associées aux profils de messagerie, notamment sur le traitement de la présence de profils existants et la suppression de profils de messagerie, consultez [Ajouter des paramètres de courrier aux appareils à l’aide de Intune](https://docs.microsoft.com/intune/email-settings-configure).

Pour plus d’informations sur la création de profils de messagerie pour chaque plateforme d’appareil, consultez :

[Paramètres de l’appareil Android pour configurer le courrier, l’authentification et la synchronisation dans Intune](https://docs.microsoft.com/intune/email-settings-android)  
[ Ajouter les paramètres de courrier électronique pour les appareils iOS et iPadOS dans Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Paramètres de profil de messagerie dans Microsoft Intune pour les appareils exécutant Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Paramètres de profil de messagerie pour les appareils exécutant Windows 10 dans Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Problème de synchronisation courants**

**L’utilisation d’un profil de messagerie KNOX sur Android empêche les contacts, le calendrier et les tâches de se synchroniser avec les appareils utilisateur.**

Le profil de courriel KNOX sur Android KNOX offre à l'administrateur la possibilité de décider quels types de contenu sont synchronisés avec l'appareil en définissant chacun sur activé.

Si le paramètre de n’importe quel type de contenu est défini sur **Non configuré** (valeur par défaut), ce type de contenu n’est pas synchronisé automatiquement. Un utilisateur peut activer le type de contenu qu’il souhaite utiliser directement sur l’appareil manuellement, mais cette configuration est remplacée par le paramètre de stratégie Intune, et la synchronisation s’arrête pour ce type de contenu.

