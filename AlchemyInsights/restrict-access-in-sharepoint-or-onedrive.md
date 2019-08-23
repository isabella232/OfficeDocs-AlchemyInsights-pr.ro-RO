---
title: Restricţiona accesul în SharePoint sau OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551463"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="2f111-102">Restricţiona accesul în SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="2f111-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="2f111-103">În SharePoint şi OneDrive, vă restricţiona accesul la elemente ca fişiere, foldere şi listelor de acordare acces numai la grupuri sau persoane care doriţi să aibă acces.</span><span class="sxs-lookup"><span data-stu-id="2f111-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="2f111-104">În mod implicit, permisiuni în SharePoint sunt moștenite de la mai sus în ierarhia.</span><span class="sxs-lookup"><span data-stu-id="2f111-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="2f111-105">Deci un fişier moștenește permisiuni sale de la folderul care moștenește permisiuni sale de la biblioteca, care moștenește permisiuni sale de la site-ul.</span><span class="sxs-lookup"><span data-stu-id="2f111-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="2f111-106">Aveţi posibilitatea să partajaţi la un nivel superior (cum ar fi prin schimbul de un întreg site-ul) şi apoi rupe moştenire, în cazul în care nu doriţi să partajaţi toate elementele de pe site-ul.</span><span class="sxs-lookup"><span data-stu-id="2f111-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="2f111-107">Cu toate acestea, nu recomandăm acest lucru pentru că face mentinerea permisiuni mai complexe şi confuze în viitor.</span><span class="sxs-lookup"><span data-stu-id="2f111-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="2f111-108">Aici este ceea ce ai putea face în schimb:</span><span class="sxs-lookup"><span data-stu-id="2f111-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="2f111-109">În cazul în care, de exemplu, doriţi să partajaţi toate conţinutul unui folder cu excepţia un fişier în ea, mutaţi fişierul respectiv într-o locaţie nouă, care nu este partajat.</span><span class="sxs-lookup"><span data-stu-id="2f111-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="2f111-110">Dacă aveţi două subfoldere într-un folder, şi doriţi să partajaţi un subfolder cu grupele A și B şi permite doar Grupa A acces la al doilea subdosar, partajaţi folderul părinte cu Grupa A şi adăugaţi grupa B la primul subfolder.</span><span class="sxs-lookup"><span data-stu-id="2f111-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="2f111-111">Opri partajarea unui fişier sau folder</span><span class="sxs-lookup"><span data-stu-id="2f111-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

