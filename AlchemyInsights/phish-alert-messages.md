---
title: 2491 Mesajele de e-mail de avertizare de la politica "Mesaje de e-mail livrate ca urmare a entității găzduite sau a înlocuirii utilizatorului"
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544590"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="5c4a5-102">Mesaje de e-mail de avertizare de la politica "Mesaje livrate cu mesaje de e-mail trimise prin entitatea găzduită sau înlocuirea utilizatorilor"</span><span class="sxs-lookup"><span data-stu-id="5c4a5-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="5c4a5-103">O politică de avertizare implicită, numită "Livrat anterior datorită entității găzduite sau înlocuirii utilizatorilor", a fost trimisă către entitățile găzduite cu Microsoft Defender pentru licențele Office 365 P1 și P2.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="5c4a5-104">Dacă ați primit această avertizare, iată pașii pentru a investiga:</span><span class="sxs-lookup"><span data-stu-id="5c4a5-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="5c4a5-105">Din mesajul de avertizare, faceți **clic pe Vizualizare** avertizare pentru a vă **duce** la pagina Avertizări din Centrul de & conformitate.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="5c4a5-106">Selectați avertizarea pentru a vedea opțiunea vizualizarea **listei de mesaje** sau **Vizualizarea mesajelor în Explorer.**</span><span class="sxs-lookup"><span data-stu-id="5c4a5-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="5c4a5-107">Ambele opțiuni vă duc la detaliile mesajului, care include ID-ul de mesaj.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="5c4a5-108">Rețineți că linkul Threat Explorer va filtra automat mesajele care se potrivesc cu criteriile de avertizare.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="5c4a5-109">Poate fi necesar să ajustați filtrul de dată în Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="5c4a5-110">Mesajul de înșelăciune a fost livrat din cauza unei înlocuiri configurate manual:</span><span class="sxs-lookup"><span data-stu-id="5c4a5-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="5c4a5-111">Un expeditor sau un domeniu permis setat de utilizator.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="5c4a5-112">Un expeditor sau un domeniu permis setate de administrator într-o politică antispam.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="5c4a5-113">O adresă IP permisă într-o politică de filtrare a conexiunii.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="5c4a5-114">O regulă de flux de corespondență (numită și regulă de transport) care este configurată pentru a permite mesajele.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="5c4a5-115">În cazul în care credeți că mesajul a fost marcat incorect ca perisator, utilizați programul de completare Outlook [de](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) raportare a mesajelor pentru a remite eșantioane de mesaje la Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5c4a5-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
