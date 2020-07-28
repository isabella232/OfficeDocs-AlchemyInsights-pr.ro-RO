---
title: Modificarea canalelor de actualizare pentru aplicațiile Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440018"
---
# <a name="change-update-channels-for-office-apps"></a>Modificarea canalelor de actualizare pentru aplicațiile Office

Pentru noile instalări Office, utilizați Setări descărcare software Office pentru a selecta canalul de actualizare dorit, apoi instalați (sau reinstalați) aplicațiile Office. Pentru mai multe informații, consultați [Gestionarea setărilor de descărcare a software-ului în Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Notă** Canalul de actualizare selectat utilizând Setările de descărcare software Office se aplică tuturor utilizatorilor care efectuează instalări noi utilizând portalul O365. Pentru mai multe informații, consultați [Descărcarea și instalarea sau reinstalarea Microsoft 365 sau Office 2019 pe un PC sau Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Pentru instalările Office existente, utilizați Instrumentul de implementare Office (ODT) pentru a comuta la un alt canal de actualizare:  

1. Descărcați cea mai recentă versiune a Instrumentului de implementare Office (setup.exe) de la [Centrul de descărcări Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identificați numele canalului la care doriți să comutați. Pentru mai multe informații, consultați [Opțiuni de configurare pentru Instrumentul de implementare Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Creați un fișier XML de configurare care specifică numele canalului corespunzător, de exemplu, update.xml.  
    R. <Configuration>  
    B. <Updates **Channel="Lunar"** />  
    C. </Configuration>
4. Dintr-un prompt de comandă ridicat, comutați la locația folderului unde se află setup.exe și executați următoarea comandă:  
    R. setup.exe /configure update.xml
5. Porniți o aplicație Office (cum ar fi Excel), apoi selectați **Cont fișier**  >  **Account**. În secțiunea Informații produs, selectați **Actualizare opțiuni**  >  **actualizare acum**.

Pentru mai multe informații, consultați [Cum se comută canalele de actualizare pentru aplicațiile Office existente](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Pentru comutarea canalelor de actualizare pentru un grup selectat de utilizatori sau utilizând Configuration Manager (SCCM), configurați setarea Update Channel utilizând GPO. Pentru mai multe informații, consultați [Prezentarea generală a canalelor de actualizare pentru aplicațiile Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Pentru detalii, consultați [Cum se gestionează canalele Office 365 ProPlus pentru profesioniști IT](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) și se [gestionează actualizările pentru aplicațiile Microsoft 365 cu Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).