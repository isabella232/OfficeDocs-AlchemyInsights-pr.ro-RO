---
title: 2491 alertați mesajele de e-mail de la politica "phishing livrate din cauza entității găzduite sau a utilizatorului"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728623"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="188ac-102">Avertizarea mesajelor de e-mail de la politica "phishing livrate din cauza entității găzduite sau a utilizatorului</span><span class="sxs-lookup"><span data-stu-id="188ac-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="188ac-103">O politică de avertizare implicită denumită "phishing livrat din cauza entității găzduite sau a unui utilizator de înlocuire" a fost lansată pentru entități găzduite cu licențe Office 365 ATP P1 și P2.</span><span class="sxs-lookup"><span data-stu-id="188ac-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="188ac-104">Dacă ați primit această avertizare, Iată pașii de investigat:</span><span class="sxs-lookup"><span data-stu-id="188ac-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="188ac-105">Din mesajul de avertizare, faceți clic pe **vizualizare avertizare** pentru a merge la pagina **avertizări** din centrul de conformitate & de securitate.</span><span class="sxs-lookup"><span data-stu-id="188ac-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="188ac-106">Selectați avertizarea pentru a vedea opțiunea de a **vizualiza lista** de mesaje sau a **vizualiza mesajele în Explorer**.</span><span class="sxs-lookup"><span data-stu-id="188ac-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="188ac-107">Ambele opțiuni vă duc la detaliile mesajului, care include ID-ul mesajului.</span><span class="sxs-lookup"><span data-stu-id="188ac-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="188ac-108">Rețineți că linkul Threat Explorer va filtra automat mesajele care se potrivește cu criteriile de avertizare.</span><span class="sxs-lookup"><span data-stu-id="188ac-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="188ac-109">Poate fi necesar să ajustați filtrul de date în Explorer.</span><span class="sxs-lookup"><span data-stu-id="188ac-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="188ac-110">Mesajul de phishing a fost livrat din cauza unei supracomenzi configurate manual:</span><span class="sxs-lookup"><span data-stu-id="188ac-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="188ac-111">Un expeditor sau un domeniu permis setat de utilizator.</span><span class="sxs-lookup"><span data-stu-id="188ac-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="188ac-112">Un expeditor sau un domeniu permis setat de administrator într-o politică anti-spam.</span><span class="sxs-lookup"><span data-stu-id="188ac-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="188ac-113">O adresă IP permisă într-o politică de filtrare a conexiunii.</span><span class="sxs-lookup"><span data-stu-id="188ac-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="188ac-114">O regulă de flux de corespondență (denumită și regulă de transport) care este configurată pentru a permite mesajele din.</span><span class="sxs-lookup"><span data-stu-id="188ac-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="188ac-115">Dacă considerați că mesajul a fost marcat incorect ca phishing, utilizați programul de [completare pentru mesaje de raport](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook pentru a trimite eșantioane de mesaje la Microsoft.</span><span class="sxs-lookup"><span data-stu-id="188ac-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
