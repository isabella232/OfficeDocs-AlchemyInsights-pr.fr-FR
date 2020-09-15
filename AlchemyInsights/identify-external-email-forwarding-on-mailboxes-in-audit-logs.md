---
title: Identifier le transfert de courrier électronique externe sur les boîtes aux lettres dans les journaux d’audit
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696295"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="b818d-102">Identifier quand le transfert de courrier électronique externe est configuré sur les boîtes aux lettres</span><span class="sxs-lookup"><span data-stu-id="b818d-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="b818d-103">Lorsqu’un utilisateur de Microsoft 365 configure le transfert de messages externes sur une boîte aux lettres, l’activité est auditée dans le cadre de la cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="b818d-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="b818d-104">Vous pouvez voir l’activité à l’aide de la recherche de journal d’audit dans le centre de sécurité & conformité.</span><span class="sxs-lookup"><span data-stu-id="b818d-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="b818d-105">Connectez-vous au [Centre de conformité & Microsoft 365 Security](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="b818d-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="b818d-106">Accédez à la **Search**  >  page de**recherche du journal d’audit** de la recherche.</span><span class="sxs-lookup"><span data-stu-id="b818d-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="b818d-107">Sélectionnez la plage de dates dans les champs **Date de début** et **Date de fin** .</span><span class="sxs-lookup"><span data-stu-id="b818d-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="b818d-108">Vous n’avez pas besoin de spécifier un nom d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b818d-108">You don't need to specify a username.</span></span> <span data-ttu-id="b818d-109">Vérifiez que le champ **activités** est défini sur **afficher les résultats pour toutes les activités**.</span><span class="sxs-lookup"><span data-stu-id="b818d-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="b818d-110">Cliquez sur **Rechercher**.</span><span class="sxs-lookup"><span data-stu-id="b818d-110">Click **Search**.</span></span>

<span data-ttu-id="b818d-111">Dans les résultats, cliquez sur **Filtrer les résultats** et tapez **Set-Mailbox** dans la zone filtre d’activité.</span><span class="sxs-lookup"><span data-stu-id="b818d-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="b818d-112">Sélectionnez un enregistrement d’audit dans les résultats.</span><span class="sxs-lookup"><span data-stu-id="b818d-112">Select an audit record in the results.</span></span> <span data-ttu-id="b818d-113">Dans la fenêtre mobile des **Détails** , cliquez sur **informations supplémentaires**.</span><span class="sxs-lookup"><span data-stu-id="b818d-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="b818d-114">Vous devez examiner les détails de chaque enregistrement d’audit pour déterminer si l’activité est liée au transfert du courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="b818d-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="b818d-115">**ObjectID**: valeur d’alias de la boîte aux lettres qui a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="b818d-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="b818d-116">**Paramètres**: _ForwardingSmtpAddress_ indique l’adresse de messagerie cible.</span><span class="sxs-lookup"><span data-stu-id="b818d-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="b818d-117">**Userid**: l’utilisateur qui a configuré le transfert du courrier électronique sur la boîte aux lettres dans le champ **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="b818d-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="b818d-118">Pour plus d’informations, consultez [la rubrique Détermination de la personne qui a configuré le transfert du courrier pour une boîte aux lettres](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="b818d-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
