---
title: Serviciul 5.7.750 1048 nu este disponibil. Client blocat de la trimiterea de la domenii neînregistrate
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664254"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="ad178-103">Clientul 5.7.750 a fost blocat din trimiterea de la un domeniu neînregistrat</span><span class="sxs-lookup"><span data-stu-id="ad178-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="ad178-104">Eroarea apare atunci când un volum mare de mesaje este trimis din domenii care nu sunt furnizate în entitatea găzduită (adăugate ca domenii acceptate și validate).</span><span class="sxs-lookup"><span data-stu-id="ad178-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="ad178-105">Pentru a evita această eroare, puteți utiliza un conector flux de corespondență bazat pe certificat, în care domeniul certificatului este un domeniu furnizat sau puteți furniza toate domeniile de trimitere.</span><span class="sxs-lookup"><span data-stu-id="ad178-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
