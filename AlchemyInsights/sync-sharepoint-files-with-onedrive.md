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
ms.openlocfilehash: 13149d288336b487441c66521b32406e408911fd
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/19/2019
ms.locfileid: "35803050"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="62592-102">Depanarea problemelor „deschidere cu Explorer“ în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="62592-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="62592-103">Comanda Deschidere cu Explorer deschide o instanță locală de Windows Explorer care afișează structura de foldere de pe serverul care găzduiește site-ul SharePoint.</span><span class="sxs-lookup"><span data-stu-id="62592-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="62592-104">Acestea fiind spuse, vă recomandăm [să sincronizați fișierele SharePoint cu noul client de sincronizare OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> care furnizează caracteristica [Fișiere la cerere](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), deoarece oferă acces local la fișiere și, implicit, performanțe optime.</span><span class="sxs-lookup"><span data-stu-id="62592-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="62592-105">Dacă ați ales să utilizați vizualizarea Explorer în loc de noul client de sincronizare OneDrive, asigurați-vă că urmați pașii și cele mai bune practici din articolele următoare:</span><span class="sxs-lookup"><span data-stu-id="62592-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="62592-106">Cum să utilizați comanda „Deschidere cu Explorer” pentru depanarea problemelor din SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="62592-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="62592-107">Copierea sau mutarea fișierelor din bibliotecă utilizând Deschidere cu Explorer</span><span class="sxs-lookup"><span data-stu-id="62592-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="62592-108">Butonul **Deschidere cu Explorer** nu apare în noua experiență de bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="62592-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="62592-109">Selectați lista verticală **Vizualizare** din dreapta sus (numele listei verticale poate diferi în funcție de vizualizarea curentă), apoi faceți clic pe **Vizualizare în Explorer**.</span><span class="sxs-lookup"><span data-stu-id="62592-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

 ><span data-ttu-id="62592-110">Funcția Deschidere cu Explorer pentru SharePoint utilizează controale ActiveX, de aceea este acceptată doar în Internet Explorer 10 sau 11.</span><span class="sxs-lookup"><span data-stu-id="62592-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="62592-111">Deschidere cu Explorer nu funcționează în Windows cu Microsoft Edge, Google Chrome, Mozilla Firefox sau pe platforma Mac.</span><span class="sxs-lookup"><span data-stu-id="62592-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="62592-112">Din acest motiv, opțiunea Vizualizare Explorer poate fi estompată.</span><span class="sxs-lookup"><span data-stu-id="62592-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

> - <span data-ttu-id="62592-113">[De ce nu sunt disponibile butoanele panglicii SharePoint sau sunt estompate](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="62592-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

