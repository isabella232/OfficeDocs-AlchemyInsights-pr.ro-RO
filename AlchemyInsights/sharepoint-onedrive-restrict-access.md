---
title: Restricționarea accesului în SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093851"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restricționarea accesului în SharePoint sau OneDrive

Există numeroase modalități de a restricționa accesul la servicii SharePoint Online/OneDrive. Aceste metode diferite de restricționare a accesului sunt descrise mai jos. 

**Restricție de permisiune**

În SharePoint Online și OneDrive pentru business, restricționăm accesul la elemente cum ar fi site-uri, fișiere și foldere, acordând acces doar acelor grupuri/persoane care ar trebui să aibă acces.

- [Particularizarea permisiunilor pentru o SharePoint sau o bibliotecă](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Particularizarea SharePoint permisiuni de site](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Modificarea permisiunilor într-un subfolder](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlul accesului de pe dispozitive necontrolate](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ca administrator SharePoint sau global, puteți să blocați sau să limitați accesul la conținutul SharePoint și OneDrive de pe dispozitive neasocate (cele care nu sunt AD hibride la care s-a alăturat sau care se conformează în Intune).

**Restricție pentru locația de rețea**

Ca administrator IT, puteți controla accesul la resursele SharePoint și OneDrive pe baza locațiilor de rețea definite în care aveți încredere. Aceasta se mai știe și sub numele de politică bazată pe locație. Pentru mai multe informații, consultați [Controlul accesului la SharePoint online și la date OneDrive bazate pe locația de rețea](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restricție de blocare site** 

În SharePoint Online, aveți posibilitatea de a bloca o colecție de site-uri, astfel încât nimeni să nu aibă acces. Acest lucru se setează prin PowerShell și prin SharePoint de administrare [Online,](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizând proprietatea [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Restricționarea creării de site-uri sau subsite-uri de către utilizatori**

Ca administrator SharePoint sau administrator global, puteți permite utilizatorilor să creeze și să-și administreze propriile site-uri SharePoint, să determine ce tip de site-uri pot să creeze și să specifice locația site-urilor. Pentru mai multe informații, consultați Gestionarea [creării site-uri în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

