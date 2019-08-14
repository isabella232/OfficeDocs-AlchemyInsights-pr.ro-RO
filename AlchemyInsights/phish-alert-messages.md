---
title: Mesaje de e-mail de alertă 2491 la politica Phish livrate din cauza locatarul sau utilizatorul suprascrie
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391468"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="ac1dc-102">Mesaje de alertă e-mail la politica Phish livrate din cauza locatarul sau utilizatorul suprascrie</span><span class="sxs-lookup"><span data-stu-id="ac1dc-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="ac1dc-103">O politică de alertă implicit numit "Phish pronunţată din cauza locatarul sau utilizatorul suprascrie" a fost rulat pentru a chiriaşilor cu Office 365 de ATP P1 şi P2 licenţe.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="ac1dc-104">În cazul în care aţi primit această avertizare, aici sunt paşii pentru a investiga:</span><span class="sxs-lookup"><span data-stu-id="ac1dc-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="ac1dc-105">Din mesajul de alertă, faceţi clic pe **Vezi alertă** pentru a merge la pagina **alerte** în securitate & centru de conformitate.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="ac1dc-106">Selectaþi Alertaþi pentru a vedea opţiunea de a **lista de mesaje Vezi** sau **vizualizarea mesajelor în Explorer**.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="ac1dc-107">Ambele aceste opţiuni vă duce la detaliile mesajului, care include identitate de mesaj.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="ac1dc-108">Reţineţi că link-ul de ameninţare Explorer automat va filtra mesajele care se potrivesc criteriilor de alertă.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="ac1dc-109">Trebuie să se adapteze filtru dată în ameninţare Explorer.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="ac1dc-110">Mesaj de înşelăciune a fost livrat din cauza o suprascrie configurat manual:</span><span class="sxs-lookup"><span data-stu-id="ac1dc-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="ac1dc-111">Un permis expeditorului sau domeniu stabilit de utilizator.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="ac1dc-112">Un permis expeditorului sau domeniu de admin în o politică anti-spam.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="ac1dc-113">O adresă IP permise într-o politică de filtru de conexiune.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="ac1dc-114">Mail fluxul de regulă (de asemenea cunoscut ca o regulă de transport) care este configurat pentru a permite mesajelor în.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="ac1dc-115">Dacă credeţi că mesajul a fost marcat incorect ca phish, utilizaţi Outlook [program de completare raport mesaj](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) să prezinte probe mesaj către Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ac1dc-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
