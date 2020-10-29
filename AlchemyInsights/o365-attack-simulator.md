---
title: 2681 Attack Simulator în Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801563"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="21022-102">Simulatorul de atac în Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="21022-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="21022-103">Vă lipsește simulatorul de atacuri?</span><span class="sxs-lookup"><span data-stu-id="21022-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="21022-104">Simulatorul de atacuri necesită **Microsoft Defender pentru office 365 plan 2 (ATP plan 2)** sau **Office 365 Enterprise E5** .</span><span class="sxs-lookup"><span data-stu-id="21022-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="21022-105">Atac Simulator **nu** este inclus în Microsoft Defender pentru Office 365 plan 1 (ATP plan 1), Office 365 Enterprise E3 sau orice aplicații Microsoft 365 pentru firme pentru abonamente.</span><span class="sxs-lookup"><span data-stu-id="21022-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="21022-106">Contul pe care îl utilizați pentru a lansa atacuri simulate necesită permisiuni de administrator global sau de administrator de securitate și autentificarea multi-factor (AMF).</span><span class="sxs-lookup"><span data-stu-id="21022-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="21022-107">Pentru mai multe informații despre cerințele pentru simulatorul de atacuri, consultați [acest subiect](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="21022-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="21022-108">Lucruri importante de știut despre simulările de atacuri cu **parolă brută Force** :</span><span class="sxs-lookup"><span data-stu-id="21022-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="21022-109">Dacă contul țintă are AMF activat și parola a fost ghicit corect, contul nu se va afișa ca compromis (al doilea factor de autentificare va fi incomplet).</span><span class="sxs-lookup"><span data-stu-id="21022-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="21022-110">Fișierul parolă nu poate fi mai mare de 10 MO.</span><span class="sxs-lookup"><span data-stu-id="21022-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="21022-111">Utilizați o parolă per linie și includeți o linie necompletată (retur transport) după ultima parolă din listă.</span><span class="sxs-lookup"><span data-stu-id="21022-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="21022-112">Lucruri importante de știut despre simulările de **înșelătorie** atașate de Lance:</span><span class="sxs-lookup"><span data-stu-id="21022-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="21022-113">Prin proiectare, nu puteți furniza o valoare particularizată pentru **URL-ul serverului de conectare la phishing** .</span><span class="sxs-lookup"><span data-stu-id="21022-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="21022-114">Dacă un destinatar utilizează programul de [completare activare mesaj raport](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) pentru a raporta mesajul ca phishing, este posibil să nu primiți avertizări pentru mesaj (deoarece acesta este un atac simulat).</span><span class="sxs-lookup"><span data-stu-id="21022-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="21022-115">Rapoarte: după finalizarea atacului simulat, puteți să faceți clic pe **Detalii despre atacuri** pentru a vedea raportul.</span><span class="sxs-lookup"><span data-stu-id="21022-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="21022-116">Pentru instrucțiuni detaliate și caracteristici noi în simulatorul de atacuri, consultați [Attack Simulator în Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="21022-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
