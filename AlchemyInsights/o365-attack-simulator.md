---
title: 2681 Simulator de atac în Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305343"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="b8427-102">Simulator de atac în Office 365</span><span class="sxs-lookup"><span data-stu-id="b8427-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="b8427-103">Iti lipseste Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="b8427-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="b8427-104">Simulator de atac necesită **Office 365 Advanced amenințare Protection Plan 2 (ATP plan 2)** sau **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="b8427-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="b8427-105">Attack Simulator **nu** este inclus în Office 365 Advanced amenințare Protection Plan 1 (ATP plan 1), Office 365 Enterprise E3, sau orice Office 365 Business abonamente.</span><span class="sxs-lookup"><span data-stu-id="b8427-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="b8427-106">Contul pe care îl utilizați pentru a lansa atacuri simulate necesită permisiuni globale de administrator sau administrator de securitate și autentificarea multi-factor (MFA).</span><span class="sxs-lookup"><span data-stu-id="b8427-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="b8427-107">Pentru mai multe informații despre cerințele de atac Simulator, consultați [acest subiect](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="b8427-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="b8427-108">Lucruri importante să știți despre **brute force parola** atac simulări:</span><span class="sxs-lookup"><span data-stu-id="b8427-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="b8427-109">Dacă contul țintă are MFA activat și parola a fost ghicit corect, contul nu va afișa ca compromis (al doilea factor de autentificare va fi incomplet).</span><span class="sxs-lookup"><span data-stu-id="b8427-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="b8427-110">Fișierul de parolă nu poate fi mai mare de 10 MB.</span><span class="sxs-lookup"><span data-stu-id="b8427-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="b8427-111">Utilizați o parolă pe linie și includeți o linie necompletată (retur transport) după ultima parolă din listă.</span><span class="sxs-lookup"><span data-stu-id="b8427-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="b8427-112">Lucruri importante de știut despre **suliță phishing** atașați simulări:</span><span class="sxs-lookup"><span data-stu-id="b8427-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="b8427-113">Prin proiectare, nu puteți furniza o valoare particularizată pentru **URL-ul serverului de conectare la phishing**.</span><span class="sxs-lookup"><span data-stu-id="b8427-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="b8427-114">Dacă un destinatar utilizează [permite Add-in raport mesaj](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) pentru a raporta mesajul ca phishing, este posibil să nu primiți alerte pentru mesaj (deoarece acesta este un atac simulat).</span><span class="sxs-lookup"><span data-stu-id="b8427-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="b8427-115">Rapoarte: după terminarea atacului simulat, puteți face clic pe **Detalii atac** pentru a vedea raportul.</span><span class="sxs-lookup"><span data-stu-id="b8427-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="b8427-116">Pentru instrucțiuni detaliate și caracteristici noi în Attack Simulator, consultați [Attack Simulator în Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="b8427-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
