---
title: Identificarea adresei IP și a clientului în jurnalele de audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508928"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="f99eb-102">Identificarea adresei IP și a clientului în jurnalele de audit</span><span class="sxs-lookup"><span data-stu-id="f99eb-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="f99eb-103">Adresa IP care corespunde unei activități de către un utilizator sau administrator Microsoft 365 este afișată în Jurnalele de audit.</span><span class="sxs-lookup"><span data-stu-id="f99eb-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="f99eb-104">Informațiile despre client sunt, de asemenea, înregistrate.</span><span class="sxs-lookup"><span data-stu-id="f99eb-104">The client information is also logged.</span></span> <span data-ttu-id="f99eb-105">Iată pașii pentru identificarea acestor informații</span><span class="sxs-lookup"><span data-stu-id="f99eb-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="f99eb-106">Conectați-vă la Centrul de [conformitate Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="f99eb-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f99eb-107">Accesați pagina **Search**  >  **de căutare în jurnalul De audit căutare.**</span><span class="sxs-lookup"><span data-stu-id="f99eb-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="f99eb-108">Dacă sunteți interesat de o anumită activitate, selectați-o din lista **Activități.**</span><span class="sxs-lookup"><span data-stu-id="f99eb-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="f99eb-109">Dacă nu, toate activitățile vor fi returnate pentru utilizatorul selectat (setare implicită).</span><span class="sxs-lookup"><span data-stu-id="f99eb-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="f99eb-110">**Notă:** Este posibil ca anumite activități să nu fie disponibile în meniul **Activități;** cu toate acestea, aceste elemente de audit vor fi returnate dacă **se afișează rezultate pentru toate activitățile** este selectat (setareimplicită).</span><span class="sxs-lookup"><span data-stu-id="f99eb-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="f99eb-111">Specificați numele de utilizator în câmpul **Utilizatori,** selectați intervalul de date corespunzător pentru activitate, apoi faceți clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="f99eb-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="f99eb-112">În rezultate, puteți vedea adresa IP pentru acea activitate în panoul de rezultate.</span><span class="sxs-lookup"><span data-stu-id="f99eb-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="f99eb-113">Selectați înregistrarea de audit pentru a vedea informații detaliate în ieșirea **Detalii** (de exemplu, Client, Utilizator care a efectuat acțiunea etc.).</span><span class="sxs-lookup"><span data-stu-id="f99eb-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="f99eb-114">Pentru mai multe informații, consultați [Găsirea adresei IP a computerului utilizat pentru a accesa un cont compromis](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="f99eb-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
