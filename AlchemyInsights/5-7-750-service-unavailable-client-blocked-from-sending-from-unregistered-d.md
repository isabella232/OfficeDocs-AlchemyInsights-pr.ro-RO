---
title: 1048 5.7.750 Service unavailable. Client blocat de la trimiterea de la domenii neînregistrate
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
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774263"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="23955-103">5.7.750 Clientul a blocat trimiterea de la domeniul neînregistrat</span><span class="sxs-lookup"><span data-stu-id="23955-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="23955-104">Eroarea apare atunci când este trimis un volum mare de mesaje de la domenii care nu sunt asigurate în entitatea găzduită (adăugate ca domenii acceptate și validate).</span><span class="sxs-lookup"><span data-stu-id="23955-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="23955-105">Pentru a evita această eroare, puteți utiliza un conector de flux de corespondență bazat pe certificat, în care domeniul certificatului este un domeniu cu acces asigurat sau puteți asigurarea accesului pentru toate domeniile de trimitere.</span><span class="sxs-lookup"><span data-stu-id="23955-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="23955-106">Pentru mai multe informații, consultați Remediați problemele de livrare a mesajelor de e-mail pentru codurile de eroare de la [5.7.700 la 5.7.750 Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span><span class="sxs-lookup"><span data-stu-id="23955-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>