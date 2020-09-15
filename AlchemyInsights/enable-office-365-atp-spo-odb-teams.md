---
title: Activarea Office 365 ATP pentru SharePoint, OneDrive și Microsoft teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709919"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activarea protecției avansate a amenințărilor Office 365 pentru SharePoint Online, OneDrive și Microsoft teams

1. Accesați https://protection.office.com și conectați-vă.
2. Alegeți Politica de **gestionare a amenințărilor**  >  **Policy**  >  **atașări sigure**.
3. Selectați **activați ATP pentru SharePoint, OneDrive și Microsoft teams**, apoi faceți clic pe **Salvare**.
4. Recomandate Ca administrator global sau administrator SharePoint Online, rulează cmdletul [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cu parametrul **DisallowInfectedFileDownload** setat la *True*.
5. Recomandate [Configurați avertizări](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pentru fișierele detectate.

> [!NOTE]
> ATP va scana fiecare fișier din SharePoint Online, OneDrive sau Microsoft teams. Fișierele sunt scanate asincron, printr-un proces care utilizează evenimente de partajare și de activitate ale invitaților, împreună cu euristica inteligentă și semnalele de amenințare pentru a identifica fișiere periculoase. Consultați [ATP pentru SharePoint, OneDrive și Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).