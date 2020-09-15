---
title: Identificarea adresei IP și a clientului în jurnalele de auditare
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668322"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="8f794-102">Identificarea adresei IP și a clientului în jurnalele de auditare</span><span class="sxs-lookup"><span data-stu-id="8f794-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="8f794-103">Adresa IP care corespunde unei activități de către un utilizator sau administrator Microsoft 365 este afișată în jurnalele de auditare.</span><span class="sxs-lookup"><span data-stu-id="8f794-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="8f794-104">Informațiile clientului sunt, de asemenea, înregistrate.</span><span class="sxs-lookup"><span data-stu-id="8f794-104">The client information is also logged.</span></span> <span data-ttu-id="8f794-105">Iată pașii pentru identificarea acestor informații</span><span class="sxs-lookup"><span data-stu-id="8f794-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="8f794-106">Conectați-vă la [Centrul de conformitate Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="8f794-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="8f794-107">Accesați **Search**  >  pagina**Căutare în Jurnalul de auditare** căutare.</span><span class="sxs-lookup"><span data-stu-id="8f794-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="8f794-108">Dacă sunteți interesat de o anumită activitate, selectați-o din lista de **activități** .</span><span class="sxs-lookup"><span data-stu-id="8f794-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="8f794-109">Dacă nu, toate activitățile vor fi returnate pentru utilizatorul selectat (setarea implicită).</span><span class="sxs-lookup"><span data-stu-id="8f794-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="8f794-110">**Notă**: este posibil ca anumite activități să nu fie disponibile în meniul **activități** ; cu toate acestea, acele elemente de audit vor fi returnate dacă se selectează **Afișare rezultate pentru toate activitățile** (setare implicită).</span><span class="sxs-lookup"><span data-stu-id="8f794-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="8f794-111">Specificați numele de utilizator în câmpul **utilizatori** , selectați intervalul de date corespunzător pentru activitate, apoi faceți clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="8f794-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="8f794-112">În rezultate, puteți vedea adresa IP pentru acea activitate în panoul rezultate.</span><span class="sxs-lookup"><span data-stu-id="8f794-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="8f794-113">Selectați înregistrarea de audit pentru a vedea informații detaliate în **detaliile** flyout (de exemplu, client, utilizator care a efectuat acțiunea etc.).</span><span class="sxs-lookup"><span data-stu-id="8f794-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="8f794-114">Pentru mai multe informații, consultați [Găsirea adresei IP a computerului utilizat pentru a accesa un cont compromis](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="8f794-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
