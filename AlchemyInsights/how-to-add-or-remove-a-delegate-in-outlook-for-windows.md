---
title: Cum se adaugă sau se elimină un delegat în Outlook pentru Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573573"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="c94fa-102">Cum se adaugă sau se elimină un delegat în Outlook pentru Windows</span><span class="sxs-lookup"><span data-stu-id="c94fa-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="c94fa-103">Pentru a adăuga un delegat în Outlook pentru Windows:</span><span class="sxs-lookup"><span data-stu-id="c94fa-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="c94fa-104">Faceți clic pe fila **fișier** , urmată de **setările contului**, apoi alegeți **delegare acces**.</span><span class="sxs-lookup"><span data-stu-id="c94fa-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="c94fa-105">Faceți clic pe **Adăugare**.</span><span class="sxs-lookup"><span data-stu-id="c94fa-105">Click on **Add**.</span></span> <span data-ttu-id="c94fa-106">Dacă **Add** nu apare, este posibil să nu existe o conexiune activă între Outlook și Exchange.</span><span class="sxs-lookup"><span data-stu-id="c94fa-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="c94fa-107">Bara de stare Outlook afișează starea conexiunii.</span><span class="sxs-lookup"><span data-stu-id="c94fa-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="c94fa-108">Tastați numele persoanei pe care doriți să o desemnați ca delegat sau căutați și alegeți numele în lista cu rezultatele căutării.</span><span class="sxs-lookup"><span data-stu-id="c94fa-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c94fa-109">Delegatul trebuie să fie o persoană din lista globală de adrese Exchange a Organizației (GAL).</span><span class="sxs-lookup"><span data-stu-id="c94fa-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="c94fa-110">Faceți clic pe **Add** urmat de **OK**.</span><span class="sxs-lookup"><span data-stu-id="c94fa-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="c94fa-111">În caseta de dialog **permisiuni delegat** , acceptați setările implicite de permisiune sau selectați niveluri de acces particularizate pentru folderele Exchange.</span><span class="sxs-lookup"><span data-stu-id="c94fa-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="c94fa-112">Dacă un delegat are nevoie de permisiune pentru a lucra doar cu solicitările de întâlnire și răspunsurile, setările de permisiune implicite, cum ar fi **delegat, primesc copii ale mesajelor asociate întâlnirii** sunt suficiente.</span><span class="sxs-lookup"><span data-stu-id="c94fa-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="c94fa-113">Puteți să lăsați setarea permisiune **Inbox** la **fără**.</span><span class="sxs-lookup"><span data-stu-id="c94fa-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="c94fa-114">Solicitările de întâlnire și răspunsurile vor merge direct la Inbox-ul delegat-ului.</span><span class="sxs-lookup"><span data-stu-id="c94fa-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c94fa-115">În mod implicit, delegatul i se acordă **Editor (poate să citească, să creeze și să modifice elemente)** în folderul **Calendar** .</span><span class="sxs-lookup"><span data-stu-id="c94fa-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="c94fa-116">Atunci când delegat răspunde la o întâlnire în numele dvs., acesta este adăugat automat în folderul **Calendar** .</span><span class="sxs-lookup"><span data-stu-id="c94fa-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="c94fa-117">Pentru a trimite un mesaj pentru a notifica delegatul pentru permisiunile modificate, bifați caseta de selectare se **trimite automat un mesaj către delegare rezumând aceste permisiuni** .</span><span class="sxs-lookup"><span data-stu-id="c94fa-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="c94fa-118">Dacă doriți, bifați caseta de selectare **delegatul poate vedea elementele mele private** .</span><span class="sxs-lookup"><span data-stu-id="c94fa-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="c94fa-119">Această setare afectează toate folderele Exchange.</span><span class="sxs-lookup"><span data-stu-id="c94fa-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="c94fa-120">Aceasta include toate folderele de corespondență, persoane de contact, calendar, activități, note și jurnal.</span><span class="sxs-lookup"><span data-stu-id="c94fa-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="c94fa-121">Nu există nicio modalitate de a acorda acces la elemente personale doar în folderele specificate.</span><span class="sxs-lookup"><span data-stu-id="c94fa-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="c94fa-122">Alegeți **OK**.</span><span class="sxs-lookup"><span data-stu-id="c94fa-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="c94fa-123">Mesajele trimise cu permisiuni trimitere în numele includ atât delegatul, cât și numele de lângă **from**.</span><span class="sxs-lookup"><span data-stu-id="c94fa-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="c94fa-124">Atunci când un mesaj este trimis cu permisiuni trimitere ca, se afișează doar numele dvs.</span><span class="sxs-lookup"><span data-stu-id="c94fa-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="c94fa-125">După ce adăugați o persoană ca delegat, aceștia pot adăuga cutia poștală Exchange la profilul Outlook.</span><span class="sxs-lookup"><span data-stu-id="c94fa-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="c94fa-126">Pentru instrucțiuni, consultați [gestionarea corespondenței și a elementelor de calendar ale altei persoane](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="c94fa-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="c94fa-127">Pentru a elimina un delegat în Outlook pentru Windows:</span><span class="sxs-lookup"><span data-stu-id="c94fa-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="c94fa-128">Faceți clic pe fila **fișier** .</span><span class="sxs-lookup"><span data-stu-id="c94fa-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="c94fa-129">Faceți clic pe **Setări cont** , urmat de **delegare acces**.</span><span class="sxs-lookup"><span data-stu-id="c94fa-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="c94fa-130">Alegeți numele delegatului pentru care doriți să modificați permisiunile, apoi faceți clic pe **Eliminare** , urmat de **OK**.</span><span class="sxs-lookup"><span data-stu-id="c94fa-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
