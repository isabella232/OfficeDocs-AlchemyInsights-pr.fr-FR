---
title: 'Scanneur AIP : installation et configuration'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934255"
---
# <a name="aip-scanner-installation-and-configuration"></a>Scanneur AIP : installation et configuration

**Pour installer le scanneur AIP, suivez les recommandations** :

1. Si vous procédez à une mise à niveau et ne procédez pas à une installation propre, veuillez vous assurer que vous avez suivi les directives pour la [mise à niveau du scanner Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) et pour le client d'étiquetage unifié, consultez la section [Mise à niveau du scanner Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Vérifiez que vous respectez la configuration requise pour tous les [Pare-feu et configuration de l’infrastructure réseau](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Assurez-vous que vos [stratégies sont définies](https://docs.microsoft.com/azure/information-protection/configure-policy) sur l’étiquetage automatique ou une étiquette par défaut dans la stratégie.
4. Assurez-vous que le type de fichier approprié est configuré pour l’étiquette/la protection, comme décrit dans [Types de fichiers pris en charge par le client Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). De plus, si vous voulez modifier le comportement par défaut, suivez ces instructions : [Modifier le niveau de protection par défaut des fichiers](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Vérifiez que le compte d’utilisateur configuré pour exécuter le service de scanneur dispose des autorisations d’accès à tous les référentiels configurés.
6. Si vous rencontrez encore des problèmes, veuillez exporter les journaux de l’analyseur et les ajouter à votre ticket de support.

**Exporter des journaux de l’analyseur Azure Information Protection**

1. Accédez à %localappdata%\Microsoft\MSIP sous le contexte utilisateur exécutant le service de numérisation.
2. Compressez tout le contenu sous le dossier MSIP.
3. Enregistrez les journaux à l’emplacement de votre choix et joignez-les à votre demande de service.
4. Vous pouvez également utiliser [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Pour plus d’informations, consultez** :
- [Déploiement du scanner Azure Information Protection pour classifier et protéger automatiquement des fichiers](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Spécifier et utiliser le paramètre de jeton pour Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Exécuter un cycle de découverte et afficher les rapports pour le scanneur](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Consultez la documentation sur Azure information protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Configuration requise pour Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Télécharger l’application Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
