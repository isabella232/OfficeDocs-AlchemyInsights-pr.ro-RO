---
title: Outlook desktop amintesc sau înlocui un mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496123"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="140f1-102">Retragerea sau înlocuirea unui mesaj de e-mail Outlook</span><span class="sxs-lookup"><span data-stu-id="140f1-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="140f1-103">Ca admin, puteți **aminti mesaje în numele utilizatorilor folosind PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="140f1-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="140f1-104">Nu vă puteți aminti mesajele de la centrul de administrare.</span><span class="sxs-lookup"><span data-stu-id="140f1-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="140f1-105">Puteți **aminti doar mesajele care sunt trimise către persoane din organizația dvs**.</span><span class="sxs-lookup"><span data-stu-id="140f1-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="140f1-106">Dacă mesajul a fost trimis la o adresă Gmail, de exemplu, nu vă puteți aminti.</span><span class="sxs-lookup"><span data-stu-id="140f1-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="140f1-107">Puteți **aminti doar mesajele trimise din Outlook 2016 pe PC**.</span><span class="sxs-lookup"><span data-stu-id="140f1-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="140f1-108">Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu vă puteți aminti.</span><span class="sxs-lookup"><span data-stu-id="140f1-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="140f1-109">Pentru a rechema sau a înlocui un mesaj e-mail:</span><span class="sxs-lookup"><span data-stu-id="140f1-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="140f1-110">În panoul de foldere din partea stângă a ferestrei Outlook, selectați folderul Elemente trimise.</span><span class="sxs-lookup"><span data-stu-id="140f1-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="140f1-111">Faceți dublu clic pe mesajul pe care doriți să-l reamintiți pentru a-l deschide.</span><span class="sxs-lookup"><span data-stu-id="140f1-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="140f1-112">Selectați fila **mesaj** , apoi selectați **acțiuni** > **reamintiți acest mesaj**.</span><span class="sxs-lookup"><span data-stu-id="140f1-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="140f1-113">Selectați **ștergeți copiile necitite ale acestui mesaj** sau **ștergeți copiile necitite și înlocuiți cu un mesaj nou**, apoi selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="140f1-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="140f1-114">Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.</span><span class="sxs-lookup"><span data-stu-id="140f1-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="140f1-115">Succesul sau eșecul unui mesaj de retragere depinde de setările destinatarului în Outlook.</span><span class="sxs-lookup"><span data-stu-id="140f1-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="140f1-116">Pentru pași pentru a verifica pe Recall, a se vedea [acest articol](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="140f1-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="140f1-117">Căutați și ștergeți mesajele de e-mail din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="140f1-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="140f1-118">Dacă nu sunteți administrator global, contul trebuie adăugat la rolul eDiscovery Manager sau la rolul de gestionare a căutării de conformitate pentru a căuta mesaje.</span><span class="sxs-lookup"><span data-stu-id="140f1-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="140f1-119">Pentru a șterge mesajele, va trebui să vă alăturați grupului de roluri Gestionare organizație sau rolului de gestionare căutare și Golire.</span><span class="sxs-lookup"><span data-stu-id="140f1-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="140f1-120">Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate și conformitate](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="140f1-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="140f1-121">[Creați o căutare de conținut](https://docs.microsoft.com/office365/securitycompliance/content-search) pentru a găsi mesajul de șters.</span><span class="sxs-lookup"><span data-stu-id="140f1-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="140f1-122">[Conectați-vă la centrul de securitate și conformitate PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="140f1-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="140f1-123">Dacă utilizați autentificarea multi-factor, consultați [conectarea la Office 365 securitate și centrul de conformitate PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="140f1-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>