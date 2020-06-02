---
title: Activarea Office 365 ATP pentru SharePoint, OneDrive și Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506930"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activarea protecției avansate pentru amenințări Office 365 pentru SharePoint Online, OneDrive și Microsoft Teams

1. Du-te https://protection.office.com și autentifică-te.
2. Alegeți **Threat management**  >  **Policy**  >  **Atașări sigure**pentru politica de gestionare a amenințărilor .
3. Selectați **Activare ATP pentru SharePoint, OneDrive și Microsoft Teams**, apoi faceți clic pe **Salvare**.
4. (Recomandat) Ca administrator global sau administrator SharePoint Online, executați cmdletul [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cu parametrul **DisallowInfectedFileDownload** setat la *true*.
5. (Recomandat) [Configurați alerte](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pentru fișierele detectate.

> [!NOTE]
> ATP va scana fiecare fișier din SharePoint Online, OneDrive sau Microsoft Teams. Fișierele sunt scanate asincron, printr-un proces care utilizează partajarea și evenimentele de activitate clienților, împreună cu euristica inteligentă și semnalele de amenințare pentru a identifica fișierele rău intenționate. Consultați [ATP pentru SharePoint, OneDrive și Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).