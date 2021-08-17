---
title: Activarea Seif atașări pentru SharePoint Online, OneDrive alte Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894475"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activarea Seif atașări pentru SharePoint Online, OneDrive alte Microsoft Teams

1. Utilizând acreditările de administrator global sau de administrator de securitate, deschideți portalul Microsoft 365 Defender la , apoi accesați Politici & reguli Politici de <https://security.microsoft.com>  \>  \> **amenințare Seif**  Atașări în secțiunea Politici

   Pentru a merge direct la **pagina Seif Atașări,** utilizați <https://security.microsoft.com/safeattachmentv2> .

2. Pe pagina **Seif Atașări,** faceți clic **pe Setări globale.**
3. În cadrul diapozitivelor imprimate care apare, selectați Activați Microsoft Defender pentru Office 365 pentru **SharePoint, OneDrive și Microsoft Teams**, apoi selectați **Salvare**.

    > [!TIP]
    >
    > Urmați acești pași pentru a îmbunătăți protecția atașărilor Seif pentru SharePoint, OneDrive și Microsoft Teams:
    >
    > - Pentru a împiedica utilizatorii să descarce fișiere rău-intenționate, utilizați valoarea pentru parametrul `$true` *DisallowInfectedFileDownload* din cmdletul **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** în SharePoint Online PowerShell. Pentru mai multe informații, consultați Utilizarea SharePoint PowerShell Online pentru a [împiedica utilizatorii să descarce fișiere rău intenționate.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    > - [Crearea unei politici de avertizare pentru fișierele detectate](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Pentru mai multe informații, Seif consultați Atașările [Office 365 pentru SharePoint, OneDrive și Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
