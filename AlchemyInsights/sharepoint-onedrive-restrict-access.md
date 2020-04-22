---
title: Restricționarea accesului în SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692777"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restricționarea accesului în SharePoint sau OneDrive

Există multe modalități de a restricționa accesul la serviciile SharePoint Online/OneDrive. Aceste diferite metode de restricționare a accesului sunt prezentate mai jos. 

**Restricționare permisiune**

În SharePoint Online și OneDrive for Business, restricționăm accesul la elemente precum site-uri, fișiere și foldere, acordând acces numai la acele grupuri/persoane care ar trebui să aibă acces.

- [Particularizarea permisiunilor pentru o listă sau o bibliotecă SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Particularizarea permisiunilor de site SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Modificarea permisiunilor pentru un subfolder](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlul accesului de la dispozitive negestionate](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ca administrator SharePoint sau global, puteți bloca sau limita accesul la conținutul SharePoint și OneDrive de pe dispozitive negestionate (cele care nu sunt asociate sau conforme cu AD hibrid în Intune).

**Restricționare locație rețea**

Ca administrator IT, puteți controla accesul la resursele SharePoint și OneDrive pe baza locațiilor de rețea definite în care aveți încredere. Aceasta este cunoscută și sub numele de politică bazată pe locație. Pentru mai multe informații, consultați [Controlul accesului la datele SharePoint Online și OneDrive bazate pe locația de rețea](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restricționare blocare site** 

În SharePoint Online aveți posibilitatea de a bloca o colecție de site-uri, astfel încât nimeni să nu aibă acces. Acest lucru este setată prin PowerShell și [Componentă de administrare SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizând proprietatea [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Restricționarea utilizatorilor de la crearea de site-uri sau subsite-uri**

Ca administrator SharePoint sau administrator global, puteți permite utilizatorilor să creeze și să administreze propriile site-uri SharePoint, să determine ce fel de site-uri pot crea și să specificați locația site-urilor. Pentru mai multe informații, consultați [Gestionarea creării site-ului în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

