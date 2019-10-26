---
title: Retransmisia e-mailului prin Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: e971593b7a67e1bb40243fc762bace6b87a35741
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745409"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="af691-102">Configurați un dispozitiv multifuncțional sau o aplicație pentru a trimite mesaje de e-mail utilizând Office 365</span><span class="sxs-lookup"><span data-stu-id="af691-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="af691-103">Pentru a afla opțiunile și pașii, consultați [Cum să configurați un dispozitiv multifuncțional sau o aplicație pentru a trimite mesaje de e-mail utilizând Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="af691-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="af691-104">**Notă:** dacă aveți un dispozitiv sau o aplicație care recent a încetat să funcționeze, vă rugăm să rețineți că am început recent [să dezactivăm cifrul 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption), conform planificării.</span><span class="sxs-lookup"><span data-stu-id="af691-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="af691-105">Pentru a vedea dispozitivele afectate, accesați [Raportul clienților cu autentificare SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="af691-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="af691-106">Erorile uzuale ar putea fi similare cu: Eroarea de autentificare, Eroarea TLS, Eroarea algoritmului de cifrare, Nepotrivirea de algoritm sau Conexiunea abandonată.</span><span class="sxs-lookup"><span data-stu-id="af691-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="af691-107">Pentru a rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="af691-107">To resolve the issue:</span></span>
 - <span data-ttu-id="af691-108">**Windows Server 2003 IIS SMTP nu va mai funcționa - este necesară o versiune mai nouă de Windows.**</span><span class="sxs-lookup"><span data-stu-id="af691-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="af691-109">Consultați furnizorul aplicației sau al dispozitivului pentru a vedea dacă este acceptat un cifru modern sau dacă există o actualizare.</span><span class="sxs-lookup"><span data-stu-id="af691-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
