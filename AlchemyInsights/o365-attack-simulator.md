---
title: 2681 Attack Liga în Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545738"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="b44e5-102">Atac Arădoare în Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b44e5-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="b44e5-103">Ratați Atac 365?</span><span class="sxs-lookup"><span data-stu-id="b44e5-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="b44e5-104">Attack Attack requires **Microsoft Defender for Office 365 Plan 2** or Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="b44e5-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="b44e5-105">Liga nu este **inclus** în Microsoft Defender pentru Office 365 Plan 1, Office 365 Enterprise E3 sau în Aplicații Microsoft 365 pentru afaceri abonamente.</span><span class="sxs-lookup"><span data-stu-id="b44e5-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="b44e5-106">Contul pe care îl utilizați pentru a lansa atacuri simulate necesită permisiuni de administrator global sau de administrator de securitate și autentificare multi-factor (MFA).</span><span class="sxs-lookup"><span data-stu-id="b44e5-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="b44e5-107">Pentru mai multe informații despre cerințele pentru atacurile din sua, [consultați acest articol.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="b44e5-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="b44e5-108">Aspecte importante de știt despre **simularea atacurilor** de tip Forță brută a parolelor:</span><span class="sxs-lookup"><span data-stu-id="b44e5-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="b44e5-109">În cazul în care contul țintă are activată autentificarea MFA și parola a fost ghicită corect, contul nu se va afișa ca compromis (al doilea factor de autentificare va fi incomplet).</span><span class="sxs-lookup"><span data-stu-id="b44e5-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="b44e5-110">Fișierul parolă nu poate fi mai mare de 10 MB.</span><span class="sxs-lookup"><span data-stu-id="b44e5-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="b44e5-111">Utilizați o parolă pentru fiecare linie și includeți o linie necompletată (returnare linie) după ultima parolă din listă.</span><span class="sxs-lookup"><span data-stu-id="b44e5-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="b44e5-112">Aspecte importante de spus despre **simularea atașării de phishing:**</span><span class="sxs-lookup"><span data-stu-id="b44e5-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="b44e5-113">Prin proiectare, nu puteți furniza o valoare particularizată pentru **URL-ul de server de conectare la phishing.**</span><span class="sxs-lookup"><span data-stu-id="b44e5-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="b44e5-114">Dacă un destinatar [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) utilizează programul de completare Activare mesaj raport pentru a raporta mesajul ca phishing, este posibil să nu primiți avertizări pentru mesaj (deoarece este un atac simulat).</span><span class="sxs-lookup"><span data-stu-id="b44e5-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="b44e5-115">Rapoarte: După terminarea atacului simulat, puteți face clic pe Detalii **atac** pentru a vedea raportul.</span><span class="sxs-lookup"><span data-stu-id="b44e5-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="b44e5-116">Pentru instrucțiuni detaliate și caracteristici noi în Atac 2010, [consultați Atac A se află în Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="b44e5-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
