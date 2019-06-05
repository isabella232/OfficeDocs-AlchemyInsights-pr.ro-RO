---
title: Depanați mesajele de acces refuzat
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716658"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Depanarea Access Denied mesaje în centrul de administrare Sharepoint/OneDrive

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Dacă vi se administrează un accent denied mesaj atunci când încearcă să navigaţi la un centru de administrare Sharepoint/OneDrive, vă rugăm să asiguraţi-vă că vă <a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">atribuiţi o licenţă de utilizator </a>. În cazul în care utilizatorul are o licenta, de asemenea, ar trebui să asiguraţi-vă că acestea se <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">atribuie un rol de administrator</a> care poate accesa centrele de admin.</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Această problemă poate apărea când un utilizator este şters şi re-creat cu acelaşi nume principal de utilizator (UPN). Noul cont este creat folosind o valoare diferită de PUID (paşaport unic ID). Atunci când utilizatorul încearcă să acceseze o colecţie de site-ul sau lor OneDrive, utilizatorul are un PUID incorecte. Un al doilea scenariu implică sincronizare director cu o unitate organizaţională de Active Directory (OU). În cazul în care utilizatorii au deja conectat la SharePoint, apoi sa mutat la un OU diferite şi resynced cu SharePoint, acestea se pot confrunta aceasta problema.</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Pentru a rezolva această problemă, trebuie să restabiliţi UPN original cu paşii din articol, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">restaura un utilizator în Office 365</a>.</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">Notă:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">în cazul în care un centru de OneDrive sau administrator SharePoint nu este disponibil pentru mai mulţi utilizatori care anterior a avut acces, poate fi o problemă temporară serviciu.&nbsp; </span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"> <a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">Verifica tabloul de sănătate serviciu</span></a>.</span></em></span></span></p>


