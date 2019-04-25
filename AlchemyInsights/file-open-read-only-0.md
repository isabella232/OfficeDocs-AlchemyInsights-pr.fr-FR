---
title: Fichier ouvert en lecture seule
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: be232b682b7bb3d24f59ad10501edbd796e6bcaf
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401751"
---
# <a name="file-open-read-only"></a><span data-ttu-id="89d15-102">Fichier ouvert en lecture seule</span><span class="sxs-lookup"><span data-stu-id="89d15-102">File open read-only</span></span>

<span data-ttu-id="89d15-103">Vous pouvez constater que lorsque vous ouvrez des fichiers, ils s'ouvrent en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="89d15-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="89d15-104">Dans certains cas, il s'agit d'une sécurité supplémentaire, par exemple lorsque vous ouvrez des fichiers à partir d'Internet et d'autres fois, il peut être dû à un paramètre pouvant être modifié.</span><span class="sxs-lookup"><span data-stu-id="89d15-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="89d15-105">Voici quelques scénarios dans lesquels un fichier s'ouvre en lecture seule et des étapes que vous pouvez suivre pour le modifier.</span><span class="sxs-lookup"><span data-stu-id="89d15-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="89d15-106">**Mon antivirus est à l'origine de l'ouverture en lecture seule**</span><span class="sxs-lookup"><span data-stu-id="89d15-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="89d15-107">Certains programmes antivirus peuvent vous protéger contre les fichiers potentiellement dangereux en les ouvrant en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="89d15-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="89d15-108">Vous devrez peut-être consulter votre fournisseur d'antivirus pour savoir comment ajuster ces paramètres.</span><span class="sxs-lookup"><span data-stu-id="89d15-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="89d15-109">BitDefender, par exemple, comporte du contenu sur l'ajout d'exclusions d'applications ici: [comment ajouter des exclusions d'applications ou de processus dans le centre de contrôle BitDefender](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="89d15-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="89d15-110">**Les propriétés de fichier sont-elles définies en lecture seule?**</span><span class="sxs-lookup"><span data-stu-id="89d15-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="89d15-111">Vous pouvez vérifier les propriétés du fichier en cliquant avec le bouton droit sur le fichier et en choisissant Propriétés.</span><span class="sxs-lookup"><span data-stu-id="89d15-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="89d15-112">Si l'attribut lecture seule est activé, vous pouvez le décocher et cliquer sur OK.</span><span class="sxs-lookup"><span data-stu-id="89d15-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="89d15-113">**Le contenu est en mode protégé**</span><span class="sxs-lookup"><span data-stu-id="89d15-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="89d15-114">Les fichiers provenant d'Internet et d'autres emplacements potentiellement dangereux peuvent contenir des virus, des vers ou d'autres types de programmes malveillants qui peuvent endommager votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="89d15-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="89d15-115">Cela est également le cas pour les pièces jointes ou les fichiers que vous avez téléchargés.</span><span class="sxs-lookup"><span data-stu-id="89d15-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="89d15-116">Pour vous aider à protéger votre ordinateur, les fichiers de ces emplacements potentiellement dangereux sont ouverts en mode protégé.</span><span class="sxs-lookup"><span data-stu-id="89d15-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="89d15-117">En utilisant le mode protégé, vous pouvez lire un fichier et afficher son contenu tout en réduisant les risques.</span><span class="sxs-lookup"><span data-stu-id="89d15-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="89d15-118">Pour plus d'informations sur le mode protégé et sur la façon de modifier les paramètres, consultez cet article: [qu'est-ce que le mode protégé?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="89d15-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="89d15-119">**OneDrive est-il plein?**</span><span class="sxs-lookup"><span data-stu-id="89d15-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="89d15-120">Si le fichier est stocké sur OneDrive et que votre espace de stockage OneDrive est plein, vous ne pourrez pas enregistrer le document tant que vous n'aurez pas sous votre espace alloué.</span><span class="sxs-lookup"><span data-stu-id="89d15-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="89d15-121">Vous pouvez vérifier votre espace libre sur OneDrive en cliquant sur l'icône OneDrive dans le centre de notification et en sélectionnant gérer le stockage, [http://onedrive.live.com](http://onedrive.live.com)ou vous pouvez accéder à, vous connecter et noter la quantité d'espace utilisé dans le coin inférieur gauche de l'écran.</span><span class="sxs-lookup"><span data-stu-id="89d15-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="89d15-122">**Office est-il activé?**</span><span class="sxs-lookup"><span data-stu-id="89d15-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="89d15-123">Si Office n'est pas activé, ou si votre abonnement a expiré, il se peut que vous soyez en mode de fonctionnalité réduite en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="89d15-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="89d15-124">Pour plus d'informations sur l'activation d'Office, consultez la rubrique suivante: Unlicensed [Product and activation Errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="89d15-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="89d15-125">**Si tout le reste échoue...**</span><span class="sxs-lookup"><span data-stu-id="89d15-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="89d15-126">Essayez de redémarrer l'ordinateur.</span><span class="sxs-lookup"><span data-stu-id="89d15-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="89d15-127">Installer les mises à jour d'Office</span><span class="sxs-lookup"><span data-stu-id="89d15-127">Install Office updates</span></span>
    
- <span data-ttu-id="89d15-128">Effectuer une réparation en ligne d'Office</span><span class="sxs-lookup"><span data-stu-id="89d15-128">Perform an Online repair of Office</span></span>
    

