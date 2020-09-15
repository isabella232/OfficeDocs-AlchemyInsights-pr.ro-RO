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
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700467"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restricționarea accesului în SharePoint sau OneDrive

Există mai multe modalități de a restricționa accesul la serviciile SharePoint Online/OneDrive. Aceste diverse metode de restricționare a accesului sunt prezentate mai jos. 

**Restricție de permisiune**

În SharePoint Online și OneDrive pentru Business, restricționăm accesul la elemente cum ar fi site-uri, fișiere și foldere prin acordarea accesului doar la acele grupuri/persoane care ar trebui să aibă acces.

- [Particularizarea permisiunilor pentru o listă sau o bibliotecă SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Particularizarea permisiunilor de site SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Modificarea permisiunilor pentru un subfolder](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlul accesului de pe dispozitive negestionate](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

În calitate de administrator SharePoint sau global, puteți să blocați sau să limitați accesul la conținut SharePoint și OneDrive de pe dispozitive negestionate (acele reclame hibride care nu sunt asociate sau compatibile în Intune).

**Restricție de locație de rețea**

Ca administrator IT, puteți să controlați accesul la resursele SharePoint și OneDrive pe baza locațiilor de rețea definite în care aveți încredere. Acest lucru este cunoscut și ca politică bazată pe locație. Pentru mai multe informații, consultați [controlul accesului la date SharePoint Online și OneDrive pe baza locației rețelei](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restricție de blocare a site-ului** 

În SharePoint Online, aveți capacitatea de a bloca o colecție de site-uri, pentru ca nimeni să nu aibă acces. Acest lucru este setat prin PowerShell și în [componenta de administrare SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizând proprietatea [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Restricționarea utilizatorilor de la crearea de site-uri sau subsite-uri**

Ca administrator SharePoint sau administrator global, puteți permite utilizatorilor să creeze și să administreze propriile site-uri SharePoint, să stabilească ce tipuri de site-uri pot crea și să specifice locația site-urilor. Pentru mai multe informații, consultați [gestionarea creării site-urilor în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

