---
title: Asistența Microsoft Edge pentru Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584013"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="a4cf6-102">Asistența Microsoft Edge pentru Microsoft Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="a4cf6-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="a4cf6-103">Proiectat pentru Windows 10 și Microsoft Edge, Guard Application utilizează o abordare de izolare hardware care permite unui utilizator să navigheze pe un site care nu este de încredere din interiorul unui container izolat, Hyper-V-enabled, separat de sistemul de operare gazdă.</span><span class="sxs-lookup"><span data-stu-id="a4cf6-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="a4cf6-104">Un administrator de întreprindere definește o listă de site-uri web de încredere, resurse cloud și rețele interne.</span><span class="sxs-lookup"><span data-stu-id="a4cf6-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="a4cf6-105">Atunci când un utilizator vizitează un site care nu se află în listă, Microsoft Edge va deschide site-ul în container.</span><span class="sxs-lookup"><span data-stu-id="a4cf6-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="a4cf6-106">Acest lucru înseamnă că, dacă site-ul se dovedește a fi rău intenționat, PC-ul gazdă va rămâne protejat, iar atacatorul nu va accesa datele întreprinderii.</span><span class="sxs-lookup"><span data-stu-id="a4cf6-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="a4cf6-107">Instalarea extensiilor în container este acceptată de Microsoft Edge Version 81 și poate fi controlată prin intermediul unei politici.</span><span class="sxs-lookup"><span data-stu-id="a4cf6-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="a4cf6-108">Adresa updateURL care se utilizează în politica ExtensionInstallForcelist ar trebui să fie adăugată ca resursă neutră în politicile de izolare a rețelei utilizate de Garda de aplicații.</span><span class="sxs-lookup"><span data-stu-id="a4cf6-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="a4cf6-109">Pentru mai multe informații, consultați [asistența Microsoft Edge pentru Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="a4cf6-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
