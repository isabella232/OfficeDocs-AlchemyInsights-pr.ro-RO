---
title: Controlul actualizărilor automate pentru aplicațiile Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439922"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="ef383-102">Controlul actualizărilor automate pentru aplicațiile Office</span><span class="sxs-lookup"><span data-stu-id="ef383-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="ef383-103">În mod implicit, actualizările pentru Aplicații Office sunt descărcate automat și aplicate în fundal, fără nicio intervenție a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="ef383-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="ef383-104">Cu toate acestea, administratorii pot controla modul în care se aplică actualizările utilizând setările Office Update.</span><span class="sxs-lookup"><span data-stu-id="ef383-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="ef383-105">Setările de actualizare permit administratorilor să activeze sau să dezactiveze actualizările automate, să afișeze sau să ascundă butonul **Actualizare acum** în Office, să seteze termene de actualizare și multe altele.</span><span class="sxs-lookup"><span data-stu-id="ef383-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="ef383-106">Pentru informații detaliate, consultați:</span><span class="sxs-lookup"><span data-stu-id="ef383-106">For detailed information, see:</span></span>

- [<span data-ttu-id="ef383-107">Configurarea setărilor de actualizare pentru Office</span><span class="sxs-lookup"><span data-stu-id="ef383-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="ef383-108">Actualizarea automată pentru Office nu este activată</span><span class="sxs-lookup"><span data-stu-id="ef383-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="ef383-109">Definirea modului de actualizare a Office după instalare</span><span class="sxs-lookup"><span data-stu-id="ef383-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="ef383-110">Pentru a revizui setările de actualizări existente aplicate unui computer client, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="ef383-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="ef383-111">Deschideți Registry Editor accesând **Start**  >  **Run**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="ef383-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="ef383-112">Comutați la următoarea locație și revizuiți setările Office Update:</span><span class="sxs-lookup"><span data-stu-id="ef383-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="ef383-113">R.</span><span class="sxs-lookup"><span data-stu-id="ef383-113">a.</span></span> <span data-ttu-id="ef383-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="ef383-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="ef383-115">B.</span><span class="sxs-lookup"><span data-stu-id="ef383-115">b.</span></span> <span data-ttu-id="ef383-116">Faceți clic peToRun\Configurare</span><span class="sxs-lookup"><span data-stu-id="ef383-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="ef383-117">**Notă**  Dacă este setată cheia OfficeMgmtCOM, este posibil să vedeți mesajul "Actualizările sunt gestionate de administratorul de sistem" în Actualizări **Office**  >  **Account**  >  **Office**.</span><span class="sxs-lookup"><span data-stu-id="ef383-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="ef383-118">Pentru mai multe informații, consultați [Gestionarea actualizărilor pentru aplicațiile Microsoft 365 cu Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="ef383-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  