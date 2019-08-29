---
title: S/MIME în Outlook pe web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666852"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="8e9dc-102">Criptaţi mesajele de e-mail în Outlook</span><span class="sxs-lookup"><span data-stu-id="8e9dc-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="8e9dc-103">Criptare de mesaj Office 365 este construit pe Microsoft Azure administrarea drepturilor (RMS azuriu), care face parte din protecția informațiilor cu Azure.</span><span class="sxs-lookup"><span data-stu-id="8e9dc-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="8e9dc-104">În cazul în care abonamentul include Azure Rights Management sau protecția informațiilor Azure, **nu aveţi nevoie să ia orice măsuri pentru a activa manual sau activa** şi serviciul de gestionare a drepturilor.</span><span class="sxs-lookup"><span data-stu-id="8e9dc-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="8e9dc-105">Bazat pe feedback-ul clientului, ne va nu mai fi care să permită Exchange mail fluxul reguli să cripteze automat outbound e-mail care conţine anumit tip de informaţii sensibile în chiriaşul dumneavoastră în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="8e9dc-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="8e9dc-106">În schimb, ne oferă instrucţiuni detaliate pe cum pot face acest lucru singuri.</span><span class="sxs-lookup"><span data-stu-id="8e9dc-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="8e9dc-107">Pentru detalii suplimentare despre cum să creaţi o regulă de transport pentru a cripta datele sensibile, a se vedea [acest articol](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="8e9dc-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="8e9dc-108">Dacă utilizaţi Outlook pe Web (fostă **OWA**): atunci când compuneţi un mesaj de poştă electronică, faceţi clic pe **Protejare** în OWA.</span><span class="sxs-lookup"><span data-stu-id="8e9dc-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="8e9dc-109">Aceasta se va aplica "Face nu transmite" permisiunea.</span><span class="sxs-lookup"><span data-stu-id="8e9dc-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="8e9dc-110">Faceţi clic pe **Schimbare permisiuni** şi selectaţi **criptare** pentru a cripta doar mesajul.</span><span class="sxs-lookup"><span data-stu-id="8e9dc-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="8e9dc-111">În cazul în care folosind **clientul Outlook**: pentru a expedia un mesaj criptat din Outlook 2013 sau 2016 sau Outlook 2016 pentru Mac, selectaţi **Opţiuni** > **permisiunile**, apoi selectaţi opţiunea de protecţie ce trebuie.</span><span class="sxs-lookup"><span data-stu-id="8e9dc-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="8e9dc-112">Să **cripteze automat toate e-mail** trimise unor destinatari sau organizaţiile partenere externe, trebuie să creaţi o regulă de transport a fluxului de corespondenţă în centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e9dc-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="8e9dc-113">Instrucţiuni detaliate sunt oferite în [acest articol de sprijin](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="8e9dc-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

