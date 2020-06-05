---
title: E-mailuri lipsă în carantină
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569557"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="3b3f9-102">E-mailuri lipsă în carantină"</span><span class="sxs-lookup"><span data-stu-id="3b3f9-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="3b3f9-103">Administratorii pot [vizualiza, elibera sau șterge aceste mesaje.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="3b3f9-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="3b3f9-104">Pentru a deschide Centrul de conformitate & securitate, accesați [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="3b3f9-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="3b3f9-105">Pentru a deschide direct pagina Carantină, accesați [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="3b3f9-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="3b3f9-106">Puteți căuta după următoarele valori:</span><span class="sxs-lookup"><span data-stu-id="3b3f9-106">You can search by the following values:</span></span>  

- <span data-ttu-id="3b3f9-107">**ID mesaj:** Identificatorul unic global al mesajului.</span><span class="sxs-lookup"><span data-stu-id="3b3f9-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="3b3f9-108">Dacă selectați un mesaj în listă, valoarea **Message ID** apare în panoul de ieșire **Detalii** care apare.</span><span class="sxs-lookup"><span data-stu-id="3b3f9-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="3b3f9-109">Administratorii pot utiliza [urmărirea mesajelor](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) pentru a găsi mesajele și valorile corespunzătoare ale Message ID.</span><span class="sxs-lookup"><span data-stu-id="3b3f9-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="3b3f9-110">**Adresa de e-mail a expeditorului:** adresa de e-mail a unui singur expeditor.</span><span class="sxs-lookup"><span data-stu-id="3b3f9-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="3b3f9-111">**Adresa de e-mail a destinatarului**: adresa de e-mail a unui singur destinatar.</span><span class="sxs-lookup"><span data-stu-id="3b3f9-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="3b3f9-112">**Subiect:** Utilizați întregul subiect al mesajului.</span><span class="sxs-lookup"><span data-stu-id="3b3f9-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="3b3f9-113">Căutarea nu este sensibilă la litere mari și mici.</span><span class="sxs-lookup"><span data-stu-id="3b3f9-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="3b3f9-114">După ce ați introdus criteriile de căutare, faceți clic pe ![ Reîmprospătare ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) buton**Reîmprospătare** pentru a filtra rezultatele.  </span><span class="sxs-lookup"><span data-stu-id="3b3f9-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="3b3f9-115">Cmdleturile pe care le utilizați pentru a vizualiza și gestionează mesajele și fișierele aflate în carantină sunt:</span><span class="sxs-lookup"><span data-stu-id="3b3f9-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="3b3f9-116">Mesaj de carantină ștergere</span><span class="sxs-lookup"><span data-stu-id="3b3f9-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="3b3f9-117">Mesaj de carantină de export</span><span class="sxs-lookup"><span data-stu-id="3b3f9-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="3b3f9-118">Mesaj de carantină</span><span class="sxs-lookup"><span data-stu-id="3b3f9-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="3b3f9-119">[Preview-quarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Rețineți că acest cmdlet este numai pentru mesaje, nu fișiere malware de la ATP pentru SharePoint Online, OneDrive pentru business sau echipe.</span><span class="sxs-lookup"><span data-stu-id="3b3f9-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="3b3f9-120">Mesaj de carantină de lansare</span><span class="sxs-lookup"><span data-stu-id="3b3f9-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)