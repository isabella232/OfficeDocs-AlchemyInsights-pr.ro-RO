---
title: Retragerea sau înlocuirea unui mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353518"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="ff2e9-102">Retragerea sau înlocuirea unui mesaj de e-mail în Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ff2e9-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="ff2e9-103">Puteți să **rememorați doar mesajele care sunt trimise persoanelor din organizația dvs**.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ff2e9-104">De exemplu, dacă mesajul a fost trimis la o adresă Gmail, nu vă puteți retrage memoria.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="ff2e9-105">Puteți să **rememorați doar mesajele trimise din Outlook pentru PC**.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="ff2e9-106">Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu vă puteți retrage memoria.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="ff2e9-107">În calitate de administrator al entității găzduite, puteți să retrageți **mesaje în numele utilizatorilor, utilizând PowerShell** (pentru mai multe informații, consultați: [căutarea și ștergerea mesajelor de e-mail](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="ff2e9-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="ff2e9-108">Nu puteți retrage mesaje din centrul de administrare.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="ff2e9-109">Defilați în jos la "Căutați și ștergeți mesajele de e-mail din organizație" pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="ff2e9-110">**Retragerea sau înlocuirea unui mesaj de e-mail pe care l-ați trimis**</span><span class="sxs-lookup"><span data-stu-id="ff2e9-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="ff2e9-111">În panoul de foldere din partea stângă a ferestrei Outlook, alegeți folderul Elemente trimise.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="ff2e9-112">Deschideți mesajul pe care doriți să-l rememorați.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-112">Open the message that you want to recall.</span></span> <span data-ttu-id="ff2e9-113">Trebuie să faceți dublu clic pentru a deschide mesajul.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-113">You must double-click to open the message.</span></span> <span data-ttu-id="ff2e9-114">Selectarea mesajului astfel încât să apară în panoul de citire nu vă permite să rememorați mesajul.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="ff2e9-115">Din fila mesaj, selectați **acțiuni**  >  **retragerea acestui mesaj**.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="ff2e9-116">Alegeți **ștergeți copiile necitite ale acestui mesaj** sau **Ștergeți copii necitite și înlocuiți cu un mesaj nou**, apoi selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="ff2e9-117">Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="ff2e9-118">Succesul sau nereușita unui mesaj retras depinde de setările destinatarilor în Outlook.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="ff2e9-119">Pentru mai multe informații, inclusiv despre cum să verificați retragerea, consultați [retragerea sau înlocuirea unui mesaj de e-mail pe care l-ați trimis](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="ff2e9-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ff2e9-120">**_Pentru a căuta și a șterge mesaje de e-mail din organizația dvs_**., este mai ușor dacă sunteți administrator global. Dacă nu sunteți administrator global, contul trebuie adăugat la grupul de roluri eDiscovery Manager sau la rolul de gestionare a căutării conformității.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="ff2e9-121">Pentru a șterge mesaje, va trebui să vă asociați grupului de roluri pentru gestionarea organizației sau rolul de gestionare a căutării și eliminării.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ff2e9-122">Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate & conformitate](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ff2e9-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="ff2e9-123">[Creați o căutare de conținut](https://docs.microsoft.com/microsoft-365/compliance/content-search) pentru a găsi mesajul de șters.</span><span class="sxs-lookup"><span data-stu-id="ff2e9-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="ff2e9-124">[Conectați-vă la Security & Conformity Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ff2e9-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="ff2e9-125">Dacă utilizați Mae (multi-factor Authentication), consultați [conectarea la Microsoft 365 Security & Conformity Center PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ff2e9-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
