---
title: 1048 5.7.750 Serviciu indisponibil. Clientul blocat la trimiterea la neînregistrate de domenii
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 06be6babc524ae0d8065355218426c695f49be66
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32365874"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="5655a-103">5.7.750 client blocat la trimiterea la neînregistrate domenii</span><span class="sxs-lookup"><span data-stu-id="5655a-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="5655a-104">Eroarea apare atunci când un mare volum de mesaje sunt trimise de la domenii care nu sunt furnizate în Office 365 (adăugat ca domeniile acceptate si validate).</span><span class="sxs-lookup"><span data-stu-id="5655a-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="5655a-105">Pentru a evita această eroare, puteţi utiliza un conector de fluxul de corespondenţă pe bază de certificat în cazul în care certificatul de domeniu este un domeniu rezultant, sau vă pot asigura accesul toate domeniile trimiterea.</span><span class="sxs-lookup"><span data-stu-id="5655a-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
