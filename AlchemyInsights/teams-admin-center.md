---
title: Centre d’administration Microsoft Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670362"
---
# <a name="teams-admin-center"></a>Centre d’administration Microsoft Teams

Découvrez la gestion de Teams avec le [Centre d’administration Microsoft Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Si vous ne parvenez pas à accéder au Centre d’administration Teams, consultez les rubriques suivantes :

- Vérifiez que vous avez autorisé les [URL et adresses IP d’Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) sur les périphériques de périmètre (pare-feu, etc.) ou dans les règles de pare-feu sur votre ordinateur local.
- Vérifiez que le nom de connexion utilisé pour accéder au Portail d’administration Teams correspond à votre nom d’utilisateur répertorié sur le [Portail d’administration Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Si les utilisateurs n’apparaissent pas dans le Centre d’administration Teams, veuillez consulter :

- Avez-vous créé des utilisateurs ou attribué des licences au cours des dernières 24 heures ? Veuillez patienter au moins 24 heures avant d’ouvrir un ticket de support.
- Vérifier que vous avez attribué les licences appropriées.
- Si vous disposez d’un annuaire Active Directory local, vérifiez que [la valeur de msRTCSIP-PrimaryUserAddress ou si l’adresse SIP dans le champ ProxyAddresses de votre Active Directory local est unique et que le format correspond au](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip :**Nom d’utilisateur** de l’utilisateur dans le [Centre d’administration Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Si vous envisagez de conserver un déploiement de Skype Entreprise Server et que les utilisateurs sont hébergés en local et en ligne : suivez la **« Configuration de hybride avec Teams et Skype Entreprise Online »** dans le panneau de configuration de Skype entreprise et déplacez les utilisateurs en ligne.
