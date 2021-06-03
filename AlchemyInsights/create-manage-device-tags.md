---
title: Crearea și gestionarea etichetelor sau grupurilor de dispozitive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731965"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="f535a-102">Crearea și gestionarea etichetelor sau grupurilor de dispozitive</span><span class="sxs-lookup"><span data-stu-id="f535a-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="f535a-103">Adăugați etichete pe dispozitive pentru a crea o afiliere logică a grupului.</span><span class="sxs-lookup"><span data-stu-id="f535a-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="f535a-104">Etichetele de dispozitiv acceptă maparea corectă a rețelei, permițându-vă să atașați etichete diferite pentru a capta contextul și a activa crearea dinamică a listelor ca parte a unui incident.</span><span class="sxs-lookup"><span data-stu-id="f535a-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="f535a-105">Etichetele pot fi utilizate ca filtru în vizualizarea listă Dispozitive sau pentru a grupa dispozitivele.</span><span class="sxs-lookup"><span data-stu-id="f535a-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="f535a-106">Pentru mai multe informații despre gruparea dispozitivelor, consultați [Crearea și gestionarea etichetelor de dispozitiv.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="f535a-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="f535a-107">Puteți să adăugați etichete pe dispozitive:</span><span class="sxs-lookup"><span data-stu-id="f535a-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="f535a-108">Utilizarea portalului</span><span class="sxs-lookup"><span data-stu-id="f535a-108">Using the portal</span></span>

- <span data-ttu-id="f535a-109">Setarea unei valori pentru cheia de registry</span><span class="sxs-lookup"><span data-stu-id="f535a-109">Setting a registry key value</span></span>
 
<span data-ttu-id="f535a-110">**Notă:** Poate exista o latență între momentul adărării unei etichete pe un dispozitiv și disponibilitatea acesteia pe lista de dispozitive și pe pagina dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="f535a-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="f535a-111">Pentru a adăuga etichete de dispozitiv utilizând API, consultați [Adăugarea sau eliminarea etichetelor de dispozitiv API.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="f535a-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="f535a-112">Adăugarea și gestionarea etichetelor de dispozitiv utilizând portalul</span><span class="sxs-lookup"><span data-stu-id="f535a-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="f535a-113">Selectați dispozitivul pe care doriți să gestionați etichetele.</span><span class="sxs-lookup"><span data-stu-id="f535a-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="f535a-114">Puteți să selectați sau să căutați un dispozitiv din oricare dintre următoarele vizualizări:</span><span class="sxs-lookup"><span data-stu-id="f535a-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="f535a-115">**Tabloul de bord Cu operațiuni de securitate** Selectați numele dispozitivului din secțiunea Dispozitive de top cu avertizări active.</span><span class="sxs-lookup"><span data-stu-id="f535a-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="f535a-116">**Coadă de** avertizări - Selectați numele dispozitivului de lângă pictograma dispozitivului din coada de avertizări.</span><span class="sxs-lookup"><span data-stu-id="f535a-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="f535a-117">**Lista dispozitive** - Selectați numele dispozitivului din lista de dispozitive.</span><span class="sxs-lookup"><span data-stu-id="f535a-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="f535a-118">**Caseta căutare** - selectați Dispozitiv din meniul vertical și introduceți numele dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="f535a-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="f535a-119">De asemenea, puteți să ajungeți la pagina de avertizare prin vizualizările de fișier și IP.</span><span class="sxs-lookup"><span data-stu-id="f535a-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="f535a-120">Selectați **Gestionare** etichete din rândul cu acțiuni de răspuns.</span><span class="sxs-lookup"><span data-stu-id="f535a-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="f535a-121">Tastați pentru a găsi sau a crea etichete.</span><span class="sxs-lookup"><span data-stu-id="f535a-121">Type to find or create tags.</span></span>

<span data-ttu-id="f535a-122">Etichetele sunt adăugate la vizualizarea dispozitivului și se reflectă în vizualizarea listă Dispozitive.</span><span class="sxs-lookup"><span data-stu-id="f535a-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="f535a-123">Apoi puteți utiliza filtrul Etichete pentru a vedea lista relevantă de dispozitive.</span><span class="sxs-lookup"><span data-stu-id="f535a-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="f535a-124">Pentru mai multe informații, consultați [Crearea și gestionarea etichetelor de dispozitiv.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="f535a-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>