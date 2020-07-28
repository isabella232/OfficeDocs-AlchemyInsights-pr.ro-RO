---
title: Mai multe obiecte au aceeași adresă de e-mail ca și identitatea
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439713"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="f2353-102">Mai multe obiecte au aceeași adresă de e-mail ca și identitatea</span><span class="sxs-lookup"><span data-stu-id="f2353-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="f2353-103">**Mai multe obiecte**</span><span class="sxs-lookup"><span data-stu-id="f2353-103">**Multiple objects**</span></span>

<span data-ttu-id="f2353-104">Unul dintre motivele comune ale acestei erori este că nu se poate distribui corect o solicitare Outlook Web Access într-o prezență a mai multor obiecte care au aceeași adresă de e-mail ca și identitatea.</span><span class="sxs-lookup"><span data-stu-id="f2353-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="f2353-105">Pentru a găsi aceste obiecte, executați următoarele comenzi:</span><span class="sxs-lookup"><span data-stu-id="f2353-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="f2353-106">· Obțineți-destinatar<email address></span><span class="sxs-lookup"><span data-stu-id="f2353-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="f2353-107">· Obțineți-utilizator<email address></span><span class="sxs-lookup"><span data-stu-id="f2353-107">· Get-User <email address></span></span>

<span data-ttu-id="f2353-108">· Utilizator-get <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="f2353-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="f2353-109">· Contact-contact<email address></span><span class="sxs-lookup"><span data-stu-id="f2353-109">· Get-Contact <email address></span></span>

<span data-ttu-id="f2353-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="f2353-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="f2353-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="f2353-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="f2353-112">· Get-Mailbox <email address> -InactiveMailboxNumai</span><span class="sxs-lookup"><span data-stu-id="f2353-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="f2353-113">Pentru a rezolva problema, eliminați mai multe obiecte cu aceeași identitate de e-mail și asigurați-vă că există un singur obiect cu identitatea de e-mail specifică și că tipul său de destinatar este UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="f2353-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="f2353-114">**Aceeași adresă este utilizată pentru cutiile poștale de afaceri și de consum**</span><span class="sxs-lookup"><span data-stu-id="f2353-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="f2353-115">O altă cauză este atunci când aceeași adresă este utilizată pentru cutiile poștale de afaceri și de consum.</span><span class="sxs-lookup"><span data-stu-id="f2353-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="f2353-116">În acest caz, utilizatorul trebuie să schimbe alias lor de consum primar până când Cafe acceptă acest scenariu.</span><span class="sxs-lookup"><span data-stu-id="f2353-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="f2353-117">Aceasta este o eroare permanentă care nu dispare fără intervenție.</span><span class="sxs-lookup"><span data-stu-id="f2353-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="f2353-118">Pentru detalii, consultați [Modificarea adresei de e-mail sau a numărului de telefon pentru contul Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="f2353-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>