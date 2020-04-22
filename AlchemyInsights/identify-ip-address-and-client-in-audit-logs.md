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
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716400"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="9c767-102">Identificarea adresei IP și a clientului în jurnalele de audit</span><span class="sxs-lookup"><span data-stu-id="9c767-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="9c767-103">Adresa IP care corespunde unei activități de către un utilizator sau administrator Microsoft 365 este afișată în Jurnalele de audit.</span><span class="sxs-lookup"><span data-stu-id="9c767-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="9c767-104">Informațiile despre client sunt, de asemenea, înregistrate.</span><span class="sxs-lookup"><span data-stu-id="9c767-104">The client information is also logged.</span></span> <span data-ttu-id="9c767-105">Iată pașii pentru identificarea acestor informații</span><span class="sxs-lookup"><span data-stu-id="9c767-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="9c767-106">Conectați-vă la Centrul de [conformitate Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="9c767-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="9c767-107">Accesați pagina de căutare în jurnalul **De** > **audit căutare.**</span><span class="sxs-lookup"><span data-stu-id="9c767-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="9c767-108">Dacă sunteți interesat de o anumită activitate, selectați-o din lista **Activități.**</span><span class="sxs-lookup"><span data-stu-id="9c767-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="9c767-109">Dacă nu, toate activitățile vor fi returnate pentru utilizatorul selectat (setare implicită).</span><span class="sxs-lookup"><span data-stu-id="9c767-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="9c767-110">**Notă:** Este posibil ca anumite activități să nu fie disponibile în meniul **Activități;** cu toate acestea, aceste elemente de audit vor fi returnate dacă **se afișează rezultate pentru toate activitățile** este selectat (setareimplicită).</span><span class="sxs-lookup"><span data-stu-id="9c767-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="9c767-111">Specificați numele de utilizator în câmpul **Utilizatori,** selectați intervalul de date corespunzător pentru activitate, apoi faceți clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="9c767-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="9c767-112">În rezultate, puteți vedea adresa IP pentru acea activitate în panoul de rezultate.</span><span class="sxs-lookup"><span data-stu-id="9c767-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="9c767-113">Selectați înregistrarea de audit pentru a vedea informații detaliate în ieșirea **Detalii** (de exemplu, Client, Utilizator care a efectuat acțiunea etc.).</span><span class="sxs-lookup"><span data-stu-id="9c767-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="9c767-114">Pentru mai multe informații, consultați [Găsirea adresei IP a computerului utilizat pentru a accesa un cont compromis](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="9c767-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
