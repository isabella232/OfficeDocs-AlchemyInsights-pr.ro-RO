---
title: Mesaje de e-mail lipsă în carantină
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673726"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="b55c2-102">Mesaje de e-mail lipsă în carantină "</span><span class="sxs-lookup"><span data-stu-id="b55c2-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="b55c2-103">Administratorii pot să [vizualizeze, să lanseze sau să șteargă aceste mesaje.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="b55c2-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="b55c2-104">Pentru a deschide centrul de conformitate &, accesați [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="b55c2-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="b55c2-105">Pentru a deschide direct pagina carantină, accesați [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="b55c2-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="b55c2-106">Puteți căuta după valorile următoare:</span><span class="sxs-lookup"><span data-stu-id="b55c2-106">You can search by the following values:</span></span>  

- <span data-ttu-id="b55c2-107">**ID mesaj**: identificatorul unic global al mesajului.</span><span class="sxs-lookup"><span data-stu-id="b55c2-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="b55c2-108">Dacă selectați un mesaj în listă, valoarea  **ID mesaj**  apare în panoul flyout  **Detalii**  care apare.</span><span class="sxs-lookup"><span data-stu-id="b55c2-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="b55c2-109">Administratorii pot utiliza [urmărirea](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) mesajelor pentru a găsi mesaje și valorile corespunzătoare pentru ID-ul mesajului.</span><span class="sxs-lookup"><span data-stu-id="b55c2-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="b55c2-110">**Adresa de E-mail a expeditorului**: adresa de E-mail a unui singur expeditor.</span><span class="sxs-lookup"><span data-stu-id="b55c2-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="b55c2-111">**Adresa de E-mail a destinatarului**: adresa de E-mail a unui singur destinatar.</span><span class="sxs-lookup"><span data-stu-id="b55c2-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="b55c2-112">**Subiect**: utilizați întregul subiect al mesajului.</span><span class="sxs-lookup"><span data-stu-id="b55c2-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="b55c2-113">Căutarea nu este sensibilă la litere mari și mici.</span><span class="sxs-lookup"><span data-stu-id="b55c2-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="b55c2-114">După ce ați introdus criteriile de căutare, faceți clic pe Reîmprospătare buton reîmprospătare ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** pentru a filtra rezultatele.  </span><span class="sxs-lookup"><span data-stu-id="b55c2-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="b55c2-115">Cmdleturile pe care le utilizați pentru a vizualiza și a gestiona mesajele și fișierele în carantină sunt:</span><span class="sxs-lookup"><span data-stu-id="b55c2-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="b55c2-116">Ștergere-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b55c2-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="b55c2-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b55c2-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="b55c2-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b55c2-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="b55c2-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): rețineți că acest cmdlet este doar pentru mesaje, nu pentru fișiere malware din ATP pentru SharePoint Online, OneDrive pentru Business sau teams.</span><span class="sxs-lookup"><span data-stu-id="b55c2-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="b55c2-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b55c2-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)