---
title: Mutarea automată a mesajelor de e-mail în cutia poștală de arhivă
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527102"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="114ee-102">Mutarea automată a mesajelor de e-mail în cutia poștală de arhivă</span><span class="sxs-lookup"><span data-stu-id="114ee-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="114ee-103">Iată cum să configurați o politică pentru a muta automat e-mailul vechi al unui utilizator în cutia poștală de arhivă:</span><span class="sxs-lookup"><span data-stu-id="114ee-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="114ee-104">Accesați Arhiva [**de**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **guvernanță a datelor** de conformitate &  >   pentru a verifica dacă a fost activată o cutie poștală de arhivă pentru utilizator.</span><span class="sxs-lookup"><span data-stu-id="114ee-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="114ee-105">Dacă nu are, faceți clic pe **Activare** , apoi pe **Da** în caseta avertisment.</span><span class="sxs-lookup"><span data-stu-id="114ee-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="114ee-106">Accesați [**Centrul de administrare Exchange > gestionarea conformității > etichetele de retenție**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="114ee-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="114ee-107">Alegeți pictograma +, apoi alegeți **se aplică automat la întreaga cutie poștală**.</span><span class="sxs-lookup"><span data-stu-id="114ee-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="114ee-108">Atribuiți un nume etichetei de retenție și alegeți **Mutare în arhivă**.</span><span class="sxs-lookup"><span data-stu-id="114ee-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="114ee-109">Pentru perioada de retenție, introduceți ora dorită, cum ar fi 90 zile.</span><span class="sxs-lookup"><span data-stu-id="114ee-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="114ee-110">Faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="114ee-110">Click **Save**.</span></span>
5. <span data-ttu-id="114ee-111">Acum creați o politică de retenție: alegeți **politici de retenție**, alegeți pictograma pentru a adăuga o politică nouă.</span><span class="sxs-lookup"><span data-stu-id="114ee-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="114ee-112">Atribuiți un nume politicii de retenție, apoi faceți clic și defilați pentru a găsi și a adăuga eticheta de retenție pe care tocmai ați creat-o.</span><span class="sxs-lookup"><span data-stu-id="114ee-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="114ee-113">Faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="114ee-113">Click **Save**.</span></span>
7. <span data-ttu-id="114ee-114">În cele din urmă, aplicați Politica de retenție la cutia poștală a utilizatorului: tot în centrul de administrare Exchange, accesați  >  **cutiile poștale** destinatari.</span><span class="sxs-lookup"><span data-stu-id="114ee-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="114ee-115">Alegeți toți utilizatorii la care doriți să aplicați politica, apoi alegeți **Editare** (pictograma creion).</span><span class="sxs-lookup"><span data-stu-id="114ee-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="114ee-116">În caseta de dialog, faceți clic pe **caracteristici cutie poștală**.</span><span class="sxs-lookup"><span data-stu-id="114ee-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="114ee-117">Sub **politică de retenție**, aplicați politica pe care tocmai ați creat-o > **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="114ee-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="114ee-118">Pentru instrucțiuni pentru aplicarea politicii pentru toți utilizatorii, consultați [aplicarea unei politici de retenție la cutiile poștale](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="114ee-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
