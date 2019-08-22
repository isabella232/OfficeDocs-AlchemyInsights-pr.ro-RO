---
title: 1048 5.7.750 Serviciu indisponibil. Clientul blocat la trimiterea la neînregistrate de domenii
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 7126b4de7f7d8861afdb22af2540d6910c1d014f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494467"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="caf69-103">5.7.750 client blocat la trimiterea la neînregistrate domenii</span><span class="sxs-lookup"><span data-stu-id="caf69-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="caf69-104">Eroarea apare atunci când un mare volum de mesaje sunt trimise de la domenii care nu sunt furnizate în Office 365 (adăugat ca domeniile acceptate si validate).</span><span class="sxs-lookup"><span data-stu-id="caf69-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="caf69-105">Pentru a evita această eroare, puteţi utiliza un conector de fluxul de corespondenţă pe bază de certificat în cazul în care certificatul de domeniu este un domeniu rezultant, sau vă pot asigura accesul toate domeniile trimiterea.</span><span class="sxs-lookup"><span data-stu-id="caf69-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
