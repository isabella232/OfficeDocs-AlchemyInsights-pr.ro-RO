---
title: Importul și exportul din Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037261"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="f1873-102">Importul și exportul din Yammer</span><span class="sxs-lookup"><span data-stu-id="f1873-102">Import and export from Yammer</span></span>

<span data-ttu-id="f1873-103">**Importul**</span><span class="sxs-lookup"><span data-stu-id="f1873-103">**Import**</span></span>

<span data-ttu-id="f1873-104">Opțiunile de import pentru utilizatori variază în funcție de faptul dacă rețeaua Yammer este în [modul nativ pentru Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)sau nu.</span><span class="sxs-lookup"><span data-stu-id="f1873-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="f1873-105">**Mod non-nativ**: utilizatorii pot fi importați în grupuri utilizând [Adăugare din agendă](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (se limitează la utilizatorii 100) din setările de grup sau din rețea, utilizând [actualizarea masivă](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) din administratorul de rețea.</span><span class="sxs-lookup"><span data-stu-id="f1873-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="f1873-106">**Mod nativ**: apartenența la grup și operațiunile de apartenență la rețea ar trebui să fie efectuate de la [portalul de administrare Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)sau utilizând altă opțiune Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1873-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="f1873-107">Rețelele din modul nativ nu mai au acces la actualizarea în masă și la alte caracteristici moștenite.</span><span class="sxs-lookup"><span data-stu-id="f1873-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f1873-108">Yammer nu a acceptat niciodată importul conținutului din interiorul administratorului de rețea chiar și atunci când s-a utilizat caracteristica Export date în altă rețea.</span><span class="sxs-lookup"><span data-stu-id="f1873-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="f1873-109">Conținutul poate fi repostat de soluții pentru parteneri sau API-uri de REST Yammer.</span><span class="sxs-lookup"><span data-stu-id="f1873-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="f1873-110">**Export**</span><span class="sxs-lookup"><span data-stu-id="f1873-110">**Export**</span></span>

<span data-ttu-id="f1873-111">[Exportul datelor din rețea în cadrul administratorului de rețea](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permite exportul de conținut din rețelele Yammer, inclusiv mesaje și fișiere.</span><span class="sxs-lookup"><span data-stu-id="f1873-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="f1873-112">Atașările pot fi extrem de mari și vor determina exportul să dureze un timp semnificativ.</span><span class="sxs-lookup"><span data-stu-id="f1873-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="f1873-113">Vă recomandăm să exportați rețele active utilizând [API](https://developer.yammer.com/docs/data-export-api) -ul de export de date din bucăți după zi sau săptămână.</span><span class="sxs-lookup"><span data-stu-id="f1873-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="f1873-114">Asistența Microsoft nu furnizează scripturi particularizate în acest scop.</span><span class="sxs-lookup"><span data-stu-id="f1873-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="f1873-115">Există un [Export RGPD](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) separat pentru exportul conținutului pentru un utilizator individual.</span><span class="sxs-lookup"><span data-stu-id="f1873-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>