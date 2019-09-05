---
title: Restricționați accesul în SharePoint sau OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750676"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restricționați accesul în SharePoint sau OneDrive

Există multe modalități de a restricționa accesul la serviciile SharePoint Online/OneDrive. Aceste diferite metode de restricționare a accesului sunt prezentate mai jos. 

**Restricție permisiune**

În SharePoint Online și OneDrive for Business, restricționăm accesul la elemente ar fi site-uri, fișiere și foldere prin acordarea accesului numai la acele grupuri/persoane care ar trebui să aibă acces.

- [Particularizarea permisiunilor pentru o listă sau o bibliotecă SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Particularizarea permisiunilor de site SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Modificarea permisiunilor unui subfolder](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlul accesului de la dispozitive negestionate](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ca un SharePoint sau Global admin în Office 365, aveți posibilitatea să blocați sau să limitați accesul la conținut SharePoint și OneDrive de pe dispozitive negestionate (cei care nu hibrid AD alăturat sau conforme în Intune).

**Restricție Locație rețea**

Ca administrator IT, puteți controla accesul la resursele SharePoint și OneDrive pe baza unor locații de rețea definite în care aveți încredere. Acest lucru este cunoscut și ca politică bazată pe locație. Pentru mai multe informații, consultați [controlul accesului la datele SharePoint Online și OneDrive bazate pe locația de rețea](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restricționare blocare site** 

În SharePoint Online aveți posibilitatea de a bloca o colecție de site-uri, astfel încât nimeni nu are acces. Acest lucru este setat prin PowerShell și [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizând proprietatea [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Restricționarea utilizatorilor de crearea de site-uri sau subsite-uri**

Ca administrator SharePoint sau Office 365 global admin, puteți lăsa utilizatorii să creeze și să administreze propriile site-uri SharePoint, să determine ce fel de site-uri pot crea și să precizeze locația site-urilor. Pentru mai multe informații, consultați [gestionarea creării site-ului în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

