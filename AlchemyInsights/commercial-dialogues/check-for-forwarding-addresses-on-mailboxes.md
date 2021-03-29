---
title: Verificarea adreselor de redirecționare în cutiile poștale
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403323"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="05198-102">Verificarea adreselor de redirecționare în cutiile poștale</span><span class="sxs-lookup"><span data-stu-id="05198-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="05198-103">Uneori, hackerii redirecționează mesajele de e-mail ale utilizatorilor către ei, așadar mai întâi vom căuta adresele de redirecționare și regulile pentru cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="05198-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="05198-104">Apoi vom verifica jurnalele de auditare.</span><span class="sxs-lookup"><span data-stu-id="05198-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="05198-105">Iată cum să căutați adrese de redirecționare:</span><span class="sxs-lookup"><span data-stu-id="05198-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="05198-106">Selectați **Utilizatori**  >  **utilizatori activi.**</span><span class="sxs-lookup"><span data-stu-id="05198-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="05198-107">Selectați utilizatorul al cărui cont a fost compromis.</span><span class="sxs-lookup"><span data-stu-id="05198-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="05198-108">În meniul volant care apare, extindeți **Setări de e-mail**, apoi faceți clic **pe Editare pentru** **redirecționarea e-mailurilor**.</span><span class="sxs-lookup"><span data-stu-id="05198-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="05198-109">Eliminați toate adresele de redirecționare pe care nu le recunoașteți.</span><span class="sxs-lookup"><span data-stu-id="05198-109">Remove any forwarding addresses you don't recognize.</span></span>