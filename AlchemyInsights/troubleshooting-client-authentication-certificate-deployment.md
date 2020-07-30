---
title: Résolution des problèmes de déploiement des certificats d’authentification client
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509052"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="7a88d-102">Résolution des problèmes de déploiement des certificats d’authentification client</span><span class="sxs-lookup"><span data-stu-id="7a88d-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="7a88d-103">Les profils de certificats clients Intune NDES/SCEP et PKCS/PFX sont généralement utilisés conjointement avec d’autres types de profils tels que WiFi, VPN et e-mail pour permettre aux utilisateurs de s’authentifier auprès des ressources d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="7a88d-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="7a88d-104">Lorsque ces types de profils sont liés à un profil de certificat client dépendent du déploiement réussi de ce profil.</span><span class="sxs-lookup"><span data-stu-id="7a88d-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="7a88d-105">La configuration initiale de l’infrastructure et la configuration associée du profil de certificat client nécessitent souvent une résolution des problèmes.</span><span class="sxs-lookup"><span data-stu-id="7a88d-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="7a88d-106">Pour consulter un guide détaillé de la configuration réussie du connecteur NDES et des instructions de dépannage pour isoler les problèmes liés au déploiement de certificats, voir :</span><span class="sxs-lookup"><span data-stu-id="7a88d-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="7a88d-107">Configurer l’infrastructure pour la prise en charge de SCEP avec Intune</span><span class="sxs-lookup"><span data-stu-id="7a88d-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="7a88d-108">Vue d’ensemble de la résolution des problèmes de profils de certificats SCEP avec Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7a88d-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="7a88d-109">Utilisez les scripts PowerShell référencés pour vérifier votre configuration.</span><span class="sxs-lookup"><span data-stu-id="7a88d-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="7a88d-110">Pour plus d’informations, voir [scripts de vérification du connecteur de certificats Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="7a88d-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="7a88d-111">**Autres problèmes courants**</span><span class="sxs-lookup"><span data-stu-id="7a88d-111">**Other common issues**</span></span>

<span data-ttu-id="7a88d-112">**Lorsque j’essaie d’installer le connecteur de certificats Intune sur le serveur NDES Connector, je reçois le message «le mot de passe de la demande de certificat ne peut pas être vérifié. Elle a peut-être déjà été utilisée. Obtenez un nouveau mot de passe à envoyer avec cette demande.»**</span><span class="sxs-lookup"><span data-stu-id="7a88d-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="7a88d-113">Ce message signifie que vous devez exécuter l’installation du connecteur de certificats en tant qu’administrateur.</span><span class="sxs-lookup"><span data-stu-id="7a88d-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="7a88d-114">Dans certains environnements, les serveurs sur lesquels le certificat Intune s’exécute doivent utiliser un serveur proxy pour se connecter à Intune. par conséquent, le connecteur de certificat doit utiliser un proxy.</span><span class="sxs-lookup"><span data-stu-id="7a88d-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="7a88d-115">Dans certains cas, le connecteur NDES ignore les paramètres de proxy configurés et peut être nécessaire pour configurer les paramètres de proxy pendant l’exécution dans le contexte de sécurité LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="7a88d-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="7a88d-116">La solution consiste à exécuter Internet Explorer en tant que système et à configurer un proxy dans Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="7a88d-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="7a88d-117">Après un redémarrage du service Intune Connector, le connecteur NDES se connecte à Intune.</span><span class="sxs-lookup"><span data-stu-id="7a88d-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="7a88d-118">**Les appareils utilisateur ne reçoivent plus les certificats SCEP de NDES.**</span><span class="sxs-lookup"><span data-stu-id="7a88d-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="7a88d-119">Il est possible que le certificat d’authentification de client émis pour le serveur NDES, et spécifié lors de l’installation du connecteur NDES, ait expiré ou est manquant.</span><span class="sxs-lookup"><span data-stu-id="7a88d-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="7a88d-120">Pour résoudre :</span><span class="sxs-lookup"><span data-stu-id="7a88d-120">To resolve:</span></span> 
 
1. <span data-ttu-id="7a88d-121">Désinstallez le connecteur NDES.</span><span class="sxs-lookup"><span data-stu-id="7a88d-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="7a88d-122">Utilisez ces détails pour demander un nouveau certificat d’authentification de client ou de serveur :</span><span class="sxs-lookup"><span data-stu-id="7a88d-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="7a88d-123">Nom du sujet : CN = FQDN externe</span><span class="sxs-lookup"><span data-stu-id="7a88d-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="7a88d-124">Nom de l’autre objet (obligatoire) : DNS = nom de domaine complet (FQDN) externe, DNS = nom de domaine complet interne</span><span class="sxs-lookup"><span data-stu-id="7a88d-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="7a88d-125">Réinstallez le connecteur NDES avec le nouveau certificat.</span><span class="sxs-lookup"><span data-stu-id="7a88d-125">Reinstall the NDES connector with the new certificate.</span></span>