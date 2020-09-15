---
title: Erreur d’atténuation de l’application non détectée
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666976"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="bf23e-102">Erreur d’atténuation « l’application non détectée »</span><span class="sxs-lookup"><span data-stu-id="bf23e-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="bf23e-103">L’erreur d’installation de l’application « l’application n’a pas été détectée une fois l’installation réussie », signalée par Intune, peut se produire sur toutes les plateformes de système d’exploitation principales (Windows, iOS et Android).</span><span class="sxs-lookup"><span data-stu-id="bf23e-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="bf23e-104">Les situations les plus courantes qui génèrent cette erreur sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="bf23e-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="bf23e-105">L’application a été mise à jour en dehors de Intune (à partir d’un magasin d’applications tierce) après le déploiement initial.</span><span class="sxs-lookup"><span data-stu-id="bf23e-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="bf23e-106">Par exemple, certaines applications telles que Google Chrome peuvent effectuer des mises à jour automatiques.</span><span class="sxs-lookup"><span data-stu-id="bf23e-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="bf23e-107">Un utilisateur a désinstallé l’application après l’installation initiale.</span><span class="sxs-lookup"><span data-stu-id="bf23e-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="bf23e-108">Pour résoudre ce problème, vous devez commencer par réviser les appareils concernés afin de déterminer le scénario dans lequel l’erreur se produit.</span><span class="sxs-lookup"><span data-stu-id="bf23e-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="bf23e-109">Si l’application a été mise à jour en dehors d’Intune, le déploiement de l’application peut être configuré pour ignorer la version de l’application.</span><span class="sxs-lookup"><span data-stu-id="bf23e-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="bf23e-110">Pour ce faire, sous **Configuration de l’application > Informations sur l’application**, définir la version **Ignorer l’application** à **Oui**.</span><span class="sxs-lookup"><span data-stu-id="bf23e-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="bf23e-111">Lorsque vous ciblez le client, il peut être utile de déployer l’application en tant que « obligatoire » et de s’assurer que la dernière version est déployée.</span><span class="sxs-lookup"><span data-stu-id="bf23e-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="bf23e-112">Par ailleurs, sur la plateforme iOS, il est possible d’utiliser la fonctionnalité **autoupdate** associée au programme d’achat du volume Apple, qui peut être configuré pour effectuer une mise à jour automatique vers les nouvelles versions des applications dès qu’elles sont disponibles.</span><span class="sxs-lookup"><span data-stu-id="bf23e-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="bf23e-113">Pour plus d’informations sur la résolution des problèmes d’installation de l’application, consultez [Résoudre les problèmes d’installation d’application](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="bf23e-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
