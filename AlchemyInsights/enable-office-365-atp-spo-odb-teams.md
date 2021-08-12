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
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964645"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activați Microsoft Defender pentru Office 365 pentru SharePoint Online, pentru OneDrive, pentru Microsoft Teams

1. Mergeți https://protection.office.com la și conectați-vă.
2. Alegeți **Politică de gestionare** a  >    >  **amenințărilor Seif Atașări.**
3. Selectați **Activați Defender pentru Office 365 pentru SharePoint, OneDrive și Microsoft Teams**, apoi faceți clic pe **Salvare**.
4. (Recomandat) Ca administrator global sau administrator SharePoint Online, rulați cmdletul [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cu **DisallowInfectedFileDownload** parametrul setat la *true*.
5. (Recomandat) [Configurați avertizările](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pentru fișierele detectate.

> [!NOTE]
> Microsoft Defender pentru Office 365 va scana fiecare fișier în SharePoint Online, OneDrive sau Microsoft Teams. Fișierele sunt scanate asincron, printr-un proces care utilizează evenimente de partajare și de activitate a invitaților, împreună cu o heuristică inteligentă și semnale de amenințare pentru a identifica fișierele rău intenționate. Consultați [Microsoft Defender pentru Office 365 pentru SharePoint, OneDrive, apoi Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).