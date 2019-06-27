---
title: Depanarea problemelor „deschidere cu Explorer“ în SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: fcaca189741bd68878b1dcfab879e6e0f64e6794
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223652"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="3d335-102">Depanarea problemelor „deschidere cu Explorer“ în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="3d335-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="3d335-103">Comanda Deschidere cu Explorer deschide o instanță locală de Windows Explorer care afișează structura de foldere de pe serverul care găzduiește site-ul SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3d335-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="3d335-104">Acestea fiind spuse, vă recomandăm [să sincronizați fișierele SharePoint cu noul client de sincronizare OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> care furnizează [ fișiere la cerere](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), deoarece oferă acces local la fișiere și, implicit, performanțe optime.</span><span class="sxs-lookup"><span data-stu-id="3d335-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="3d335-105">Dacă ați ales să utilizați vizualizarea Explorer în loc de noul client de sincronizare, asigurați-vă că urmați pașii și cele mai bune practici din articolele de mai jos.</span><span class="sxs-lookup"><span data-stu-id="3d335-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="3d335-106">Cum să utilizați comanda „Deschidere cu Explorer” pentru depanarea problemelor din SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="3d335-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="3d335-107">Copierea sau mutarea fișierelor din bibliotecă utilizând Deschidere cu Explorer</span><span class="sxs-lookup"><span data-stu-id="3d335-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="3d335-108">Notă: butonul Deschidere cu Explorer nu apare în noua experiență de bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="3d335-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="3d335-109">Faceți clic pe Vizualizare listă verticală din colțul din dreapta sus (numele modificărilor verticale sunt în funcție de vizualizarea curentă), apoi faceți clic pe Vizualizare în fișierul Explorer.</span><span class="sxs-lookup"><span data-stu-id="3d335-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="3d335-110">Funcția Deschidere cu Explorer pentru SharePoint utilizează controale ActiveX, așadar este acceptată doar în Internet Explorer 10 sau 11.</span><span class="sxs-lookup"><span data-stu-id="3d335-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="3d335-111">Deschidere cu Explorer nu funcționează în Windows cu Microsoft Edge, Google Chrome, Mozilla Firefox sau pe platforma Mac.</span><span class="sxs-lookup"><span data-stu-id="3d335-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="3d335-112">Din acest motiv, opțiunea Vizualizare Explorer poate fi estompată.</span><span class="sxs-lookup"><span data-stu-id="3d335-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="3d335-113">[De ce nu sunt disponibile butoanele panglicii SharePoint sau sunt estompate](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="3d335-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

