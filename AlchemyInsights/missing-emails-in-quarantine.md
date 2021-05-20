---
title: Mesaje de e-mail lipsă în carantină
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539836"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="0212c-102">Mesaje de e-mail lipsă în carantină"</span><span class="sxs-lookup"><span data-stu-id="0212c-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="0212c-103">Administratorii pot [vizualiza, lansa sau șterge aceste mesaje.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="0212c-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="0212c-104">Pentru a deschide Centrul de & conformitate, accesați [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="0212c-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="0212c-105">Pentru a deschide direct pagina Carantină, accesați [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="0212c-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="0212c-106">Puteți să căutați după următoarele valori:</span><span class="sxs-lookup"><span data-stu-id="0212c-106">You can search by the following values:</span></span>  

- <span data-ttu-id="0212c-107">**ID mesaj:** identificatorul unic global al mesajului.</span><span class="sxs-lookup"><span data-stu-id="0212c-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="0212c-108">Dacă selectați un mesaj din listă, valoarea  **ID mesaj**  apare în panoul  **volant**  Detalii care apare.</span><span class="sxs-lookup"><span data-stu-id="0212c-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="0212c-109">Administratorii pot utiliza urmărirea [mesajelor pentru](/microsoft-365/security/office-365-security/message-trace-scc) a găsi mesajele și valorile ID-ul de mesaj corespunzătoare.</span><span class="sxs-lookup"><span data-stu-id="0212c-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="0212c-110">**Adresa de e-mail** a expeditorului: adresa de e-mail a unui singur expeditor.</span><span class="sxs-lookup"><span data-stu-id="0212c-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="0212c-111">**Adresa de e-mail** a destinatarului: adresa de e-mail a unui singur destinatar.</span><span class="sxs-lookup"><span data-stu-id="0212c-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="0212c-112">**Subiect:** Utilizați întregul subiect al mesajului.</span><span class="sxs-lookup"><span data-stu-id="0212c-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="0212c-113">Căutarea nu face sensibil la litere mari și mici.</span><span class="sxs-lookup"><span data-stu-id="0212c-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="0212c-114">După ce ați introdus criteriile de căutare, faceți clic ![ pe butonul Reîmprospătare ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **reîmprospătare** pentru a filtra rezultatele.</span><span class="sxs-lookup"><span data-stu-id="0212c-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="0212c-115">Cmdleturi pe care le utilizați pentru a vizualiza și gestiona mesajele și fișierele din carantină sunt:</span><span class="sxs-lookup"><span data-stu-id="0212c-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="0212c-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0212c-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="0212c-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0212c-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="0212c-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0212c-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="0212c-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Rețineți că acest cmdlet este doar pentru mesaje, nu pentru fișierele malware de la Microsoft Defender pentru Office 365 pentru SharePoint Online, OneDrive pentru business sau Teams.</span><span class="sxs-lookup"><span data-stu-id="0212c-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="0212c-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0212c-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)