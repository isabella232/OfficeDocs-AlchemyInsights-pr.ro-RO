---
title: Căutarea adreselor de redirecționare în cutiile poștale
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427712"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="19889-102">Căutarea adreselor de redirecționare în cutiile poștale</span><span class="sxs-lookup"><span data-stu-id="19889-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="19889-103">Uneori, hackerii redirecționează mesajele de e-mail ale utilizatorilor, astfel că mai întâi vom căuta adresele și regulile de redirecționare în cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="19889-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="19889-104">Apoi vom verifica jurnalele de auditare.</span><span class="sxs-lookup"><span data-stu-id="19889-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="19889-105">Iată cum să căutați adresele de redirecționare:</span><span class="sxs-lookup"><span data-stu-id="19889-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="19889-106">Selectați **utilizatori**  >  **activi** utilizatori.</span><span class="sxs-lookup"><span data-stu-id="19889-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="19889-107">Selectați utilizatorul al cărui cont a fost compromis.</span><span class="sxs-lookup"><span data-stu-id="19889-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="19889-108">În flyout care apare, extindeți **setările de e-mail**, apoi faceți clic pe **Editare** pentru **redirecționare e-mail**.</span><span class="sxs-lookup"><span data-stu-id="19889-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="19889-109">Eliminați toate adresele de redirecționare pe care nu le recunoașteți.</span><span class="sxs-lookup"><span data-stu-id="19889-109">Remove any forwarding addresses you don't recognize.</span></span>