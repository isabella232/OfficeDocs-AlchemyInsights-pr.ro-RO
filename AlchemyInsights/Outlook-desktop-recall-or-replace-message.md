---
title: Outlook desktop retragerea sau înlocuirea unui mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664002"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="9d7a2-102">Retragerea sau înlocuirea unui mesaj de e-mail Outlook</span><span class="sxs-lookup"><span data-stu-id="9d7a2-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="9d7a2-103">Ca administrator, puteți retrage **mesaje în numele utilizatorilor care utilizează PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="9d7a2-104">Nu puteți retrage mesaje din centrul de administrare.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="9d7a2-105">Puteți să **rememorați doar mesajele care sunt trimise persoanelor din organizația dvs**.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="9d7a2-106">În cazul în care mesajul a fost trimis la o adresă Gmail, de exemplu, nu vă puteți retrage memoria.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="9d7a2-107">Puteți să **rememorați doar mesajele trimise din Outlook 2016 pe PC**.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="9d7a2-108">Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu vă puteți retrage memoria.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="9d7a2-109">Pentru retragerea sau înlocuirea unui mesaj de e-mail:</span><span class="sxs-lookup"><span data-stu-id="9d7a2-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="9d7a2-110">În panoul de foldere din partea stângă a ferestrei Outlook, selectați folderul Elemente trimise.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="9d7a2-111">Faceți dublu clic pe mesajul pe care doriți să-l rememorați pentru a-l deschide.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="9d7a2-112">Selectați fila **mesaj** , apoi faceți clic pe **acțiuni**  >  **retragerea acestui mesaj**.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="9d7a2-113">Selectați **ștergeți copiile necitite ale acestui mesaj** sau **Ștergeți copii necitite și înlocuiți cu un mesaj nou**, apoi selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="9d7a2-114">Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="9d7a2-115">Succesul sau nereușita unui mesaj retras depinde de setările destinatarului în Outlook.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="9d7a2-116">Pentru pașii necesari pentru a verifica retragerea, consultați [acest articol](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="9d7a2-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="9d7a2-117">Căutarea și ștergerea mesajelor de e-mail din organizație</span><span class="sxs-lookup"><span data-stu-id="9d7a2-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="9d7a2-118">Dacă nu sunteți administrator global, contul dumneavoastră trebuie să fie adăugat la rolul managerului eDiscovery sau la rolul de gestionare a căutării conformității pentru a căuta mesaje.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="9d7a2-119">Pentru a șterge mesaje, va trebui să vă asociați grupului de roluri pentru gestionarea organizației sau rolul de gestionare a căutării și eliminării.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="9d7a2-120">Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate și conformitate](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="9d7a2-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="9d7a2-121">[Creați o căutare de conținut](https://docs.microsoft.com/microsoft-365/compliance/content-search) pentru a găsi mesajul de șters.</span><span class="sxs-lookup"><span data-stu-id="9d7a2-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="9d7a2-122">[Conectați-vă la centrul de securitate și conformitate PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="9d7a2-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="9d7a2-123">Dacă utilizați autentificarea multi-factor, consultați [conectarea la Microsoft 365 Security și la centrul de conformitate PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="9d7a2-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>