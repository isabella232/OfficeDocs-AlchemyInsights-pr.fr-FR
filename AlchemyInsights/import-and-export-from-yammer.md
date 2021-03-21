---
title: Importer et exporter à partir de Yammer
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
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897728"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="9b42d-102">Importer et exporter à partir de Yammer</span><span class="sxs-lookup"><span data-stu-id="9b42d-102">Import and export from Yammer</span></span>

<span data-ttu-id="9b42d-103">**Import**</span><span class="sxs-lookup"><span data-stu-id="9b42d-103">**Import**</span></span>

<span data-ttu-id="9b42d-104">Les options d’importation de l’utilisateur varient selon que votre réseau Yammer soit en [Mode natif pour Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ou non.</span><span class="sxs-lookup"><span data-stu-id="9b42d-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="9b42d-105">**Mode non natif** : les utilisateurs peuvent être importés dans des groupes à l’aide de [Ajouter à partir du carnet d’adresses](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limite à 100 utilisateurs) au sein des paramètres de groupe, ou au réseau à l’aide de [Mise à jour en bloc](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) au sein de l’administrateur réseau.</span><span class="sxs-lookup"><span data-stu-id="9b42d-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="9b42d-106">**Mode natif** : les opérations d’appartenance au groupe et d’appartenance au réseau doivent être effectuées à partir du [Portail d’administration Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [Portail Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ou à l’aide d’une autre option d’Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9b42d-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="9b42d-107">Les réseaux en mode natif n’ont plus accès à la mise à jour en bloc et à d’autres fonctionnalités héritées.</span><span class="sxs-lookup"><span data-stu-id="9b42d-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9b42d-108">Yammer n’a jamais pris en charge l’importation de contenu à partir d’un administrateur réseau même lorsque la fonctionnalité d’exportation de données était utilisée dans un autre réseau.</span><span class="sxs-lookup"><span data-stu-id="9b42d-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="9b42d-109">Le contenu peut être publié de nouveau par des solutions partenaires ou par les API Yammer REST.</span><span class="sxs-lookup"><span data-stu-id="9b42d-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="9b42d-110">**Exportation**</span><span class="sxs-lookup"><span data-stu-id="9b42d-110">**Export**</span></span>

<span data-ttu-id="9b42d-111">[L’exportation des données du réseau au sein de l’administrateur réseau](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permet d’exporter du contenu à partir de réseaux Yammer, y compris des messages et des fichiers.</span><span class="sxs-lookup"><span data-stu-id="9b42d-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="9b42d-112">Les pièces jointes peuvent être extrêmement volumineuses et entraîner des délais d'exécution importants pour les exportations.</span><span class="sxs-lookup"><span data-stu-id="9b42d-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="9b42d-113">Nous vous recommandons d’exporter des réseaux actifs à l’aide de l’[API d'exportation de données](https://developer.yammer.com/docs/data-export-api) par tranches de jours ou de semaines.</span><span class="sxs-lookup"><span data-stu-id="9b42d-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="9b42d-114">Le Support Microsoft ne fournit pas de scripts personnalisés à cet effet.</span><span class="sxs-lookup"><span data-stu-id="9b42d-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="9b42d-115">Une [exportation GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) distincte existe pour exporter le contenu pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="9b42d-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>