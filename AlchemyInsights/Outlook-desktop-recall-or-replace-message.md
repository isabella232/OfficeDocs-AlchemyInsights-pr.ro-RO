---
title: Outlook amintesc Desktop sau înlocuiţi un mesaj de e-mail
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496123"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="ea392-102">Amintesc sau să înlocuiască un mesaj de poştă electronică Outlook</span><span class="sxs-lookup"><span data-stu-id="ea392-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="ea392-103">Ca administrator, puteţi **amintesc mesaje în numele utilizatorilor folosind PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="ea392-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="ea392-104">Nu pot aminti mesaje de la centrul de administrare.</span><span class="sxs-lookup"><span data-stu-id="ea392-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="ea392-105">Puteţi **doar amintesc mesajele care sunt trimise la oameni în cadrul organizaţiei**.</span><span class="sxs-lookup"><span data-stu-id="ea392-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ea392-106">Dacă mesajul a fost trimis la o adresă de Gmail, de exemplu, tu nu pot aminti ea.</span><span class="sxs-lookup"><span data-stu-id="ea392-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="ea392-107">Puteţi **doar amintesc mesajele trimise din Outlook 2016 pe PC-ul**.</span><span class="sxs-lookup"><span data-stu-id="ea392-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="ea392-108">Dacă un utilizator trimite un mesaj cu ajutorul Outlook pentru Mac sau Outlook de pe web, tu nu-l amintesc.</span><span class="sxs-lookup"><span data-stu-id="ea392-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="ea392-109">Să-mi amintesc sau să înlocuiască un mesaj de e-mail:</span><span class="sxs-lookup"><span data-stu-id="ea392-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="ea392-110">În panoul de foldere pe partea stângă a ferestrei Outlook, selectaţi folderul Elemente trimise.</span><span class="sxs-lookup"><span data-stu-id="ea392-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="ea392-111">Faceţi dublu clic pe mesajul pe care doriţi să se amintească pentru a o deschide.</span><span class="sxs-lookup"><span data-stu-id="ea392-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="ea392-112">Selectaţi fila **mesaj** şi selectaţi **Acţiuni** > **Amintesc acest mesaj**.</span><span class="sxs-lookup"><span data-stu-id="ea392-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="ea392-113">Selectaţi **ştergeţi copiilor necitite ale acestui mesaj** sau **ştergeţi copiilor necitite și înlocuirea cu un mesaj nou**, şi apoi selectaţi **OK**.</span><span class="sxs-lookup"><span data-stu-id="ea392-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="ea392-114">Dacă sunteţi trimite un mesaj de inlocuire, compune mesajul şi selectaţi **trimite**.</span><span class="sxs-lookup"><span data-stu-id="ea392-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="ea392-115">Succesul sau eşecul de un recall de mesaj depinde de setările de destinatar în Outlook.</span><span class="sxs-lookup"><span data-stu-id="ea392-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="ea392-116">Pentru câţiva paşi pentru a verifica pe recall, a se vedea [acest articol](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="ea392-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ea392-117">Caută şi ştergeţi mesajele de e-mail în cadrul organizaţiei</span><span class="sxs-lookup"><span data-stu-id="ea392-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="ea392-118">Dacă nu sunteţi un administrator global, contul trebuie să fie adăugat rolul de Manager eDiscovery sau rol de gestionare conformitate Search pentru a căuta mesajele.</span><span class="sxs-lookup"><span data-stu-id="ea392-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="ea392-119">Pentru a ºterge mesaje, veţi avea nevoie să se alăture grupului de roluri Gestionare organizaţie sau rol de gestionare căutare și Golire.</span><span class="sxs-lookup"><span data-stu-id="ea392-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ea392-120">Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate şi de conformitate](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="ea392-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="ea392-121">[Creaţi un conţinut de căutare](https://docs.microsoft.com/office365/securitycompliance/content-search) pentru a găsi mesajul pentru a şterge.</span><span class="sxs-lookup"><span data-stu-id="ea392-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="ea392-122">[Conecta la securitatea şi conformitatea centrul PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ea392-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="ea392-123">Dacă utilizaţi autentificarea multi-factor, consultaţi [Conectare la Office 365 securitatea şi conformitatea centrul PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ea392-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>