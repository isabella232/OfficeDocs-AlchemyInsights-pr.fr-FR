---
title: Fichier ouvert en lecture seule
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813182"
---
# <a name="file-open-read-only"></a><span data-ttu-id="4485a-102">Fichier ouvert en lecture seule</span><span class="sxs-lookup"><span data-stu-id="4485a-102">File open read-only</span></span>

<span data-ttu-id="4485a-103">Vous pouvez découvrir que lorsque vous ouvrez des fichiers, ils s'ouvrent en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="4485a-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="4485a-104">Dans certains cas, il s'agit d'une sécurité supplémentaire, par exemple lorsque vous ouvrent des fichiers à partir d'Internet, et d'autres fois, cela peut être dû à un paramètre qui peut être modifié.</span><span class="sxs-lookup"><span data-stu-id="4485a-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="4485a-105">Voici quelques scénarios dans lequel un fichier s'ouvre en lecture seule et certaines étapes que vous pouvez prendre pour le modifier.</span><span class="sxs-lookup"><span data-stu-id="4485a-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="4485a-106">**Mon antivirus les entraîne à ouvrir en lecture seule.**</span><span class="sxs-lookup"><span data-stu-id="4485a-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="4485a-107">Certains programmes antivirus peuvent vous protéger contre les fichiers potentiellement dangereux en les ouvrant en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="4485a-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="4485a-108">Vous devrez peut-être consulter votre fournisseur antivirus pour savoir comment ajuster ces paramètres.</span><span class="sxs-lookup"><span data-stu-id="4485a-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="4485a-109">BitDefender, par exemple, a du contenu sur l'ajout d'exclusions d'applications ici : Comment ajouter des exclusions d'applications ou de processus dans le Centre de contrôle [Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="4485a-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="4485a-110">**Les propriétés du fichier sont-elles définies en lecture seule ?**</span><span class="sxs-lookup"><span data-stu-id="4485a-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="4485a-111">Vous pouvez vérifier les propriétés du fichier en cliquant avec le bouton droit sur le fichier et en choisissant Propriétés.</span><span class="sxs-lookup"><span data-stu-id="4485a-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="4485a-112">Si l'attribut En lecture seule est vérifié, vous pouvez le décocher et cliquer sur OK.</span><span class="sxs-lookup"><span data-stu-id="4485a-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="4485a-113">**Le contenu est en affichage protégé**</span><span class="sxs-lookup"><span data-stu-id="4485a-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="4485a-114">Les fichiers provenant d'Internet et d'autres emplacements potentiellement dangereux peuvent contenir des virus, des vers ou d'autres types de programmes malveillants susceptibles de nuire à votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="4485a-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="4485a-115">C'est également généralement le cas avec les pièces jointes ou les fichiers que vous avez téléchargés.</span><span class="sxs-lookup"><span data-stu-id="4485a-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="4485a-116">Pour protéger votre ordinateur, les fichiers de ces emplacements potentiellement dangereux sont ouverts en affichage protégé.</span><span class="sxs-lookup"><span data-stu-id="4485a-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="4485a-117">À l'aide du affichage protégé, vous pouvez lire un fichier et voir son contenu tout en réduisant les risques.</span><span class="sxs-lookup"><span data-stu-id="4485a-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="4485a-118">Pour plus d'informations sur le affichage protégé et la modification des paramètres, consultez cet article : [Qu'est-ce que le affichage protégé ?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="4485a-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="4485a-119">**OneDrive est-il plein ?**</span><span class="sxs-lookup"><span data-stu-id="4485a-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="4485a-120">Si le fichier est stocké sur OneDrive et que votre espace de stockage OneDrive est plein, vous ne pourz pas enregistrer le document tant que vous n'avez pas alloué d'espace.</span><span class="sxs-lookup"><span data-stu-id="4485a-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="4485a-121">Vous pouvez vérifier votre espace libre sur OneDrive en cliquant sur l'icône OneDrive dans le centre de notifications et en choisissant Gérer le stockage, ou vous pouvez y aller, vous connectez et notez la quantité d'espace utilisé dans la partie inférieure gauche de [https://onedrive.live.com](https://onedrive.live.com) l'écran.</span><span class="sxs-lookup"><span data-stu-id="4485a-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="4485a-122">**Office est-il activé ?**</span><span class="sxs-lookup"><span data-stu-id="4485a-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="4485a-123">Si Office n'est pas activé ou si votre abonnement a expiré, vous pouvez être en mode de fonctionnalités réduites en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="4485a-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="4485a-124">Pour plus d'informations sur l'activation d'Office, voir : Erreurs produit sans licence et [d'activation dans Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="4485a-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="4485a-125">**Si tout le reste échoue...**</span><span class="sxs-lookup"><span data-stu-id="4485a-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="4485a-126">Essayer de redémarrer l'ordinateur</span><span class="sxs-lookup"><span data-stu-id="4485a-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="4485a-127">Installer les mises à jour d’Office</span><span class="sxs-lookup"><span data-stu-id="4485a-127">Install Office updates</span></span>
    
- <span data-ttu-id="4485a-128">Effectuer une réparation en ligne d'Office</span><span class="sxs-lookup"><span data-stu-id="4485a-128">Perform an Online repair of Office</span></span>
    

