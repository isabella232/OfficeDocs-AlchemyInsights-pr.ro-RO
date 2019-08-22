---
title: Identifica adresa IP şi client în jurnalele de auditare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539041"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="0992b-102">Identifica adresa IP şi client în jurnalele de auditare</span><span class="sxs-lookup"><span data-stu-id="0992b-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="0992b-103">IP-ul care corespunde unei activități de către un utilizator Office 365 sau administratorul este indicat în jurnalele de Audit.</span><span class="sxs-lookup"><span data-stu-id="0992b-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="0992b-104">Informaţii client este, de asemenea, conectat.</span><span class="sxs-lookup"><span data-stu-id="0992b-104">The client information is also logged.</span></span> <span data-ttu-id="0992b-105">Aici sunt paşii pentru astfel de informaţii de identificare</span><span class="sxs-lookup"><span data-stu-id="0992b-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="0992b-106">Conectaţi-vă la [Centrul de conformitatea Office 365 securitate &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="0992b-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="0992b-107">Du-te la **Căutare** > pagina de**Căutare de jurnalul de Audit** .</span><span class="sxs-lookup"><span data-stu-id="0992b-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="0992b-108">Dacă sunteţi interesat într-o activitate specifică, selectaţi-l din lista de **activităţi** .</span><span class="sxs-lookup"><span data-stu-id="0992b-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="0992b-109">Dacă nu, toate activităţile vor fi returnate pentru utilizator selectat (setarea implicită).</span><span class="sxs-lookup"><span data-stu-id="0992b-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="0992b-110">**Notă**: anumite activităţi să nu fie disponibilă în meniul de **activităţi** ; cu toate acestea, cei de audit elemente vor fi returnate dacă **Arată rezultate pentru toate acțiunile** este selectat (. lipsă aranjare).</span><span class="sxs-lookup"><span data-stu-id="0992b-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="0992b-111">Specificaţi numele de utilizator în câmpul **utilizatorilor** , selectaţi intervalul de date corespunzător pentru activitatea şi apoi faceţi clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="0992b-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="0992b-112">În rezultate, puteţi vedea adresa IP pentru activitatea respectivă în panoul de rezultate.</span><span class="sxs-lookup"><span data-stu-id="0992b-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="0992b-113">Selectaţi înregistrarea de audit pentru a vedea informaţii detaliate în fișă de **Detalii** (de exemplu, Client, utilizatorul care a efectuat acţiunea, etc.).</span><span class="sxs-lookup"><span data-stu-id="0992b-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="0992b-114">Pentru informaţii suplimentare, consultaţi [Găsirea adresei IP a computerului utilizat pentru a accesa un cont compromise](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="0992b-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
