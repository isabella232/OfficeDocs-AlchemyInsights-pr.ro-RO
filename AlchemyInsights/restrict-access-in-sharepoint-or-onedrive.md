---
title: Restricţiona accesul în SharePoint sau OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485171"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="7a6ee-102">Restricţiona accesul în SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="7a6ee-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="7a6ee-p101">În SharePoint şi OneDrive, vă restricţiona accesul la elemente ca fişiere, foldere şi listelor de acordare acces numai la grupuri sau persoane care doriţi să aibă acces. În mod implicit, permisiuni în SharePoint sunt moștenite de la mai sus în ierarhia. Deci un fişier moștenește permisiuni sale de la folderul care moștenește permisiuni sale de la biblioteca, care moștenește permisiuni sale de la site-ul.</span><span class="sxs-lookup"><span data-stu-id="7a6ee-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="7a6ee-p102">Aveţi posibilitatea să partajaţi la un nivel superior (cum ar fi prin schimbul de un întreg site-ul) şi apoi rupe moştenire, în cazul în care nu doriţi să partajaţi toate elementele de pe site-ul. Cu toate acestea, nu recomandăm acest lucru pentru că face mentinerea permisiuni mai complexe şi confuze în viitor. Aici este ceea ce ai putea face în schimb:</span><span class="sxs-lookup"><span data-stu-id="7a6ee-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="7a6ee-109">În cazul în care, de exemplu, doriţi să partajaţi toate conţinutul unui folder cu excepţia un fişier în ea, mutaţi fişierul respectiv într-o locaţie nouă, care nu este partajat.</span><span class="sxs-lookup"><span data-stu-id="7a6ee-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="7a6ee-110">Dacă aveţi două subfoldere într-un folder, şi doriţi să partajaţi un subfolder cu grupele A și B şi permite doar Grupa A acces la al doilea subdosar, partajaţi folderul părinte cu Grupa A şi adăugaţi grupa B la primul subfolder.</span><span class="sxs-lookup"><span data-stu-id="7a6ee-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="7a6ee-111">Opri partajarea unui fişier sau folder</span><span class="sxs-lookup"><span data-stu-id="7a6ee-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

