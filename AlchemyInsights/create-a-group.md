---
title: Crearea unui grup
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816371"
---
# <a name="create-a-group"></a><span data-ttu-id="7e52c-102">Crearea unui grup</span><span class="sxs-lookup"><span data-stu-id="7e52c-102">Create a group</span></span>

<span data-ttu-id="7e52c-103">Acest subiect descrie crearea de grupuri.</span><span class="sxs-lookup"><span data-stu-id="7e52c-103">This topic describes group creation.</span></span>

<span data-ttu-id="7e52c-104">**Permisiunea de a crea un grup**</span><span class="sxs-lookup"><span data-stu-id="7e52c-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="7e52c-105">Asigurați-vă că sunteți autorizat să creați un grup nou.</span><span class="sxs-lookup"><span data-stu-id="7e52c-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="7e52c-106">Administratorii globali pot dezactiva crearea grupurilor în portalul Azure sau în panoul Access.</span><span class="sxs-lookup"><span data-stu-id="7e52c-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="7e52c-107">Poate fi necesar ca un administrator să creeze noul grup pentru dvs. sau să vă ofere permisiunile corespunzătoare.</span><span class="sxs-lookup"><span data-stu-id="7e52c-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="7e52c-108">**Gestionarea permisiunilor de creare a grupurilor**</span><span class="sxs-lookup"><span data-stu-id="7e52c-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="7e52c-109">Administratorii globali pot gestiona permisiunile de creare a grupurilor (din motive de securitate) sau grupurile Office 365 create în portalul Azure sau în panoul de acces, alegând opțiunile "Utilizatorii pot crea grupuri de securitate în portaluri Azure" sau "Utilizatorii pot crea grupuri Office 365 în portaluri Azure" în Toate grupurile   >  **General (Setări).**</span><span class="sxs-lookup"><span data-stu-id="7e52c-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="7e52c-110">De asemenea, puteți restricționa crearea de grupuri pentru a selecta un grup de utilizatori dacă aveți o licență Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="7e52c-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="7e52c-111">**Dezactivarea notificării de bun venit pentru noii membri ai grupului Office 365**</span><span class="sxs-lookup"><span data-stu-id="7e52c-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="7e52c-112">Notificarea de bun venit trimisă utilizatorilor care sunt adăugate la grupurile Office 365 poate fi dezactivată prin setarea **UnifiedGroupWelcomeMessageEnabled** la False în Powershell.</span><span class="sxs-lookup"><span data-stu-id="7e52c-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="7e52c-113">Aflați despre această setare [aici.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="7e52c-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

