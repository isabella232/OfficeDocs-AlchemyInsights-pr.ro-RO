---
title: 1048 5.7.750 Serviciu indisponibil. Client blocat de la trimiterea de la domenii neînregistrate
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676725"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="a49a7-103">5.7.750 Client blocat de la trimiterea de la un domeniu neînregistrat</span><span class="sxs-lookup"><span data-stu-id="a49a7-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="a49a7-104">Eroarea apare atunci când un volum mare de mesaje sunt trimise din domenii care nu sunt furnizate în entitate găzduită (adăugat ca domenii acceptate și validate).</span><span class="sxs-lookup"><span data-stu-id="a49a7-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="a49a7-105">Pentru a evita această eroare, utilizați un conector de flux de corespondență bazat pe certificat în cazul în care domeniul certificatului este un domeniu furnizat sau aveți posibilitatea să furnizați toate domeniile de trimitere.</span><span class="sxs-lookup"><span data-stu-id="a49a7-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
