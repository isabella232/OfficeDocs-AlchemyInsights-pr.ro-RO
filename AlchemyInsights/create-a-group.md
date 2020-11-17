---
title: Crearea unui grup
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089173"
---
# <a name="create-a-group"></a><span data-ttu-id="f79e4-102">Crearea unui grup</span><span class="sxs-lookup"><span data-stu-id="f79e4-102">Create a group</span></span>

<span data-ttu-id="f79e4-103">Acest subiect descrie crearea grupurilor.</span><span class="sxs-lookup"><span data-stu-id="f79e4-103">This topic describes group creation.</span></span>

<span data-ttu-id="f79e4-104">**Permisiunea de a crea un grup**</span><span class="sxs-lookup"><span data-stu-id="f79e4-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="f79e4-105">Asigurați-vă că sunteți autorizat să creați un grup nou.</span><span class="sxs-lookup"><span data-stu-id="f79e4-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="f79e4-106">Administratorii globali pot dezactiva crearea grupurilor în portalul Azure sau în panoul de acces.</span><span class="sxs-lookup"><span data-stu-id="f79e4-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="f79e4-107">Este posibil să aveți nevoie de un administrator pentru a crea noul grup sau pentru a vă oferi permisiuni corespunzătoare.</span><span class="sxs-lookup"><span data-stu-id="f79e4-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="f79e4-108">**Gestionarea permisiunilor de creare a grupurilor**</span><span class="sxs-lookup"><span data-stu-id="f79e4-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="f79e4-109">Administratorii globali pot gestiona permisiunile de creare a grupurilor (din motive legate de securitate) sau grupuri 365 Office create în portalul Azure sau în panoul de acces, alegând "utilizatorii pot crea grupuri de securitate în portaluri Azure" sau "utilizatorii pot crea grupuri Office 365 în portaluri Azure" opțiuni din **toate grupurile**  >  **generale (Setări)**.</span><span class="sxs-lookup"><span data-stu-id="f79e4-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="f79e4-110">De asemenea, puteți restricționa crearea grupurilor pentru a selecta un grup de utilizatori dacă aveți o licență Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="f79e4-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="f79e4-111">**Dezactivarea notificării de întâmpinare pentru noii membri ai grupului Office 365**</span><span class="sxs-lookup"><span data-stu-id="f79e4-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="f79e4-112">Notificarea de bun venit trimisă utilizatorilor care sunt adăugați la Office 365 Groups poate fi dezactivată setând **UnifiedGroupWelcomeMessageEnabled** la false în PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f79e4-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="f79e4-113">Aflați mai multe despre această setare [aici](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="f79e4-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

