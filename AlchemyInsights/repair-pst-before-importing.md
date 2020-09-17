---
title: Réparer le fichier. pst avant l’importation
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799094"
---
# <a name="repair-pst-file-before-importing"></a>Réparer le fichier. pst avant l’importation

Avant d’importer un fichier. pst dans Outlook, vérifiez que le fichier n’est pas endommagé en le réparant :

1. Quittez Outlook.

2. Recherchez et exécutez `Scanpst.exe` dans votre dossier de programme Office (C:\Program Files (x86) \Microsoft Office\root\Office \<Version\> ou C:\Program Files\Microsoft Office\root\Office \<Version\> ).

3. Dans l' **outil réparation de la boîte de réception Microsoft Outlook**, cliquez sur **Parcourir** pour rechercher le fichier. pst (par exemple, dans C:\Users \\<nom d’utilisateur \> \AppData\Local\Microsoft\Outlook). Sélectionnez le fichier. pst, puis cliquez sur **ouvrir**.

4. Cliquez sur **Démarrer** pour lancer l’analyse.

5. Si des erreurs sont détectées dans le fichier, cliquez sur **réparer**, puis cliquez sur **OK** une fois la réparation terminée.

6. Essayez à nouveau d’importer le fichier. pst dans Outlook.

Pour plus d’informations, consultez la rubrique [réparer les fichiers de données Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) et [corriger les problèmes lors de l’importation d’un fichier. pst Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
