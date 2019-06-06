---
title: Restricţiona accesul în SharePoint sau OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735154"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restricţiona accesul în SharePoint sau OneDrive

Există multe modalităţi de a restricţiona accesul la servicii de SharePoint Online/OneDrive. Aceste diferite metode de restricţii de acces sunt prezentate mai jos. 

Permisiunea de restricţie

În SharePoint Online şi OneDrive pentru afaceri, vom restricţiona accesul la elemente cum ar fi site-uri, fişiere şi foldere numai acorda acces la aceste grupuri/persoanele care ar trebui să aibă acces.

[Personaliza permisiuni pentru o listă SharePoint sau biblioteca](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Personaliza permisiunile de site-ul SharePoint](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[Schimba permisiunile de pe un subfolder](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Control acces la dispozitive negestionată](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

Ca SharePoint sau administrator global în Office 365, puteţi bloca sau limita accesul la conținut SharePoint și OneDrive de la negestionată dispozitive (acele nu hibrid AD s-au alăturat sau compatibil în Intune).

Restricţie de locaţie reţea

Ca un IT admin, puteţi controla accesul la resursele SharePoint și OneDrive bazat pe locațiile de rețea definită care aveţi încredere. Acest lucru este, de asemenea, cunoscut sub numele politicii bazate pe locaţie. Pentru mai multe informaţii, consultaţi [controlul accesului la SharePoint Online si OneDrive date bazate pe locaţie de reţea](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

Restricţie de blocare site-ul 

În SharePoint Online, aveţi posibilitatea de a bloca în jos o colecţie de site-ul, astfel incat nimeni nu are acces. Acest câmp este setat prin intermediul PowerShell şi [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizând proprietatea - LockState [Set-petre](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .

Limita de utilizatori la crearea de site-uri sau subsite-uri

Ca SharePoint admin sau administrator global Office 365, puteti lasa utilizatorii crea şi administra propriile site-uri SharePoint, determina ce fel de site-uri pe care le poate crea, şi specificaţi locaţia de site-uri. Pentru mai multe informaţii, vă rugăm să consultaţi [Administreaza crearea de site-ul SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)

