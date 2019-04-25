---
title: Permite ATP Office 365 pentru SharePoint, OneDrive şi Microsoft echipe
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403045"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activarea Office 365 ameninţare avansate de protecţie pentru SharePoint Online, OneDrive şi Microsoft echipe

1. Du-te la https://protection.office.com și conectați-vă.
2. Alege **Threat management** > **Politica** > **Atașări în condiţii de siguranţă**.
3. Selectați **activați ATP pentru SharePoint, OneDrive, şi echipe de Microsoft**, şi apoi faceţi clic pe **salvaţi**.
4. (Recomandat) Ca un administrator global sau un administrator de SharePoint Online, executaţi cmdlet-ul [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cu parametrul **DisallowInfectedFileDownload** setat la *adevărat*.
5. (Recomandat) [Configurarea avertizărilor](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pentru detectat fişierele.

> [!NOTE]
> ATP va nto scanare orice fişier în SharePoint Online, OneDrive sau Microsoft Teams. Fişierele sunt scanate asincron, printr-un proces care utilizează sharing şi comentariile evenimente activitatea, împreună cu smart euristică şi semnalele de ameninţare pentru a identifica fişierele rău intenţionat. A se vedea [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).