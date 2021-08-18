---
title: Activarea Office 365 ATP pentru SharePoint, OneDrive și Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4a29fdf1b61dd51b85793a1346bea193c67f70d32344470cb5449cf767da4a24
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896615"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activați Microsoft Defender pentru Office 365 pentru SharePoint Online, OneDrive aplicații și Microsoft Teams

1. Mergeți https://protection.office.com la și conectați-vă.
2. Alegeți **Politică de gestionare** a  >    >  **amenințărilor Seif Atașări.**
3. Selectați **Activați Defender pentru Office 365 pentru SharePoint, OneDrive salvare și Microsoft Teams**, apoi faceți clic pe **Salvare.**
4. (Recomandat) Ca administrator global sau SharePoint Online, rulați cmdletul [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cu **DisallowInfectedFileDownload** parametrul setat la *true*.
5. (Recomandat) [Configurați avertizările](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pentru fișierele detectate.

> [!NOTE]
> Microsoft Defender pentru Office 365 nu va scana fiecare fișier în SharePoint Online, OneDrive sau Microsoft Teams. Fișierele sunt scanate asincron, printr-un proces care utilizează evenimente de partajare și de activitate a invitaților, împreună cu o heuristică inteligentă și semnale de amenințare pentru a identifica fișierele rău intenționate. Consultați [Microsoft Defender pentru Office 365 pentru SharePoint, OneDrive, apoi Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).