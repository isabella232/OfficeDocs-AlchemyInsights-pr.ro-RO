---
title: Depanarea problemelor de încărcare a imaginilor în Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148296"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="cd287-102">Depanarea problemelor de încărcare a imaginilor în Yammer</span><span class="sxs-lookup"><span data-stu-id="cd287-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="cd287-103">Când apar probleme cu fotografiile și previzualizările de fișiere în Yammer, depanați verificând dacă problema apare pentru toți utilizatorii, dacă apare pe dispozitive mobile și dacă este reproductibilă la încărcarea atașării.</span><span class="sxs-lookup"><span data-stu-id="cd287-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="cd287-104">**Probleme cu fotografia de profil**</span><span class="sxs-lookup"><span data-stu-id="cd287-104">**Profile photo issues**</span></span>  

<span data-ttu-id="cd287-105">Dacă utilizatorii finali se conectează la Yammer prin Microsoft 365, aceștia trebuie să își schimbe profilul, inclusiv fotografia de profil.</span><span class="sxs-lookup"><span data-stu-id="cd287-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="cd287-106">Dacă utilizatorilor nu li se permite să facă actualizări de profil, un administrator poate face actualizarea pentru utilizator.</span><span class="sxs-lookup"><span data-stu-id="cd287-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="cd287-107">Pentru mai multe informații, consultați [Vizualizarea și actualizarea profilului în Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="cd287-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="cd287-108">Pentru informații despre editarea profilului, inclusiv fotografiile de profil, consultați [Modificarea profilului și setărilor Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="cd287-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="cd287-109">Fotografiile de profil actualizate sunt sincronizate diferit față de atributele de profil.</span><span class="sxs-lookup"><span data-stu-id="cd287-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="cd287-110">Utilizatorii trebuie să se conecteze pentru a iniția o sincronizare a fotografiei lor de profil.</span><span class="sxs-lookup"><span data-stu-id="cd287-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="cd287-111">Pentru informații, consultați [imaginile de profil de utilizator actualizate de la Office 365 la Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="cd287-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="cd287-112">Pentru informații despre ciclul de viață al utilizatorilor pentru Yammer, consultați [Gestionarea utilizatorilor Yammer de-a lungul ciclului lor de viață din Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="cd287-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="cd287-113">Pentru detalii despre modul în care funcționează sincronizarea imaginilor de profil în Microsoft 365, consultați [Informații despre sincronizarea imaginilor de profil în Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="cd287-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="cd287-114">**Previzualizări de documente și probleme de miniatură a imaginilor**</span><span class="sxs-lookup"><span data-stu-id="cd287-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="cd287-115">Când fișierele sau imaginile sunt postate în Yammer, este posibil ca previzualizările să nu apară, deoarece:</span><span class="sxs-lookup"><span data-stu-id="cd287-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="cd287-116">Fișierul este deteriorat și nu se poate procesa.</span><span class="sxs-lookup"><span data-stu-id="cd287-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="cd287-117">Fișierul nu a fost încărcat recent în SharePoint Online sau Yammer are metadate nevalide din alte motive.</span><span class="sxs-lookup"><span data-stu-id="cd287-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="cd287-118">URL-urile necesare pentru încărcarea imaginilor de previzualizare sunt blocate.</span><span class="sxs-lookup"><span data-stu-id="cd287-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="cd287-119">Examinarea fișierului a fost eliminată de utilizator înainte de înregistrare.</span><span class="sxs-lookup"><span data-stu-id="cd287-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="cd287-120">O problemă de serviciu a împiedicat generarea unei examinări.</span><span class="sxs-lookup"><span data-stu-id="cd287-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="cd287-121">**Notă** Este posibil ca previzualizările pentru linkuri și încărcări de fișiere să se comporte diferit.</span><span class="sxs-lookup"><span data-stu-id="cd287-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="cd287-122">Este posibil ca linkurile la fișiere de pe internet sau linkurile care necesită autentificare suplimentară să nu se afișeze corect.</span><span class="sxs-lookup"><span data-stu-id="cd287-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="cd287-123">Pentru mai multe informații, consultați [Atașarea unui fișier sau a unei imagini la un mesaj Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="cd287-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 