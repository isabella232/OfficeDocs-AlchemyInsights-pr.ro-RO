---
title: Retransmisia e-mailului prin Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117995"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="f3b9f-102">Configurați un dispozitiv multifuncțional sau o aplicație pentru a trimite mesaje de e-mail</span><span class="sxs-lookup"><span data-stu-id="f3b9f-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="f3b9f-103">Pentru a afla opțiunile și pașii, consultați [Cum să configurați un dispozitiv multifuncțional sau o aplicație pentru a trimite e-mail utilizând Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="f3b9f-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="f3b9f-104">Dacă aveți un dispozitiv sau o aplicație care nu mai funcționează recent, cele mai obișnuite probleme sunt:</span><span class="sxs-lookup"><span data-stu-id="f3b9f-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="f3b9f-105">**Erori asociate cu autentificarea în timpul utilizării remiterii clientului autentificare SMTP** Am făcut recent câteva modificări legate de modul în care funcționează autentificarea SMTP.</span><span class="sxs-lookup"><span data-stu-id="f3b9f-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="f3b9f-106">Pentru mai multe informații despre cum să rezolvați problemele, consultați secțiunea Nereușită din Remedierea problemelor cu [imprimantele, scanerele](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)și aplicațiile LOB care trimit mesaje de e-Microsoft 365 sau Office 365 .</span><span class="sxs-lookup"><span data-stu-id="f3b9f-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="f3b9f-107">**Acceptăm doar versiunea TLS 1.2 atunci când facem o conexiune sigură la Office 365** Dacă utilizați Conexiune securizată (TLS), asigurați-vă că dispozitivul dvs. de aplicație acceptă TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="f3b9f-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="f3b9f-108">Pentru mai multe informații, [consultați Pregătirea pentru TLS 1.2 în Office 365 în Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f3b9f-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="f3b9f-109">Pentru alte probleme și soluții, consultați Remedierea problemelor cu [imprimantele, scanerele](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)și aplicațiile LOB care trimit mesaje de e-mail utilizând Microsoft 365 sau Office 365 .</span><span class="sxs-lookup"><span data-stu-id="f3b9f-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="f3b9f-110">Pentru a vedea dispozitivele afectate, accesați [Raportul clienților cu autentificare SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="f3b9f-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="f3b9f-111">**Notă:** Exchange Online nu se include în scenariile de corespondență masivă.</span><span class="sxs-lookup"><span data-stu-id="f3b9f-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="f3b9f-112">Pentru a trimite e-mailuri comerciale în masă (de exemplu, buletine informative pentru clienți), trebuie să utilizați furnizori terți specializați în aceste servicii.</span><span class="sxs-lookup"><span data-stu-id="f3b9f-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
