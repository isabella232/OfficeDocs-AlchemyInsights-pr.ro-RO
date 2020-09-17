---
title: 1065 dezaprobarea adresei IP de ieșire EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806807"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="5e69e-102">Dezaprobarea zonelor de adrese IP de ieșire EOP</span><span class="sxs-lookup"><span data-stu-id="5e69e-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="5e69e-103">Am detectat o problemă potențială cu organizația dvs., care (dacă nu este corectată până la 26 octombrie 2018) poate întrerupe fluxul de corespondență la destinațiile locale sau externe.</span><span class="sxs-lookup"><span data-stu-id="5e69e-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="5e69e-104">Așa cum s-a comunicat anterior, pentru a simplifica gestionarea intervalelor de adrese IP, sintetizăm intervalele de adrese IP Exchange Online Protection (EOP) care sunt utilizate pentru a trimite și a primi mesaje de e-mail în afara Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5e69e-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="5e69e-105">Analiza noastră indică faptul că una sau mai multe dintre sursele sau destinațiile externe de e-mail pe care le-ați configurat în conectorii fluxului de corespondență nu acceptă conexiuni din intervalele de adrese IP afișate [aici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5e69e-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="5e69e-106">Acționeze înainte de 26 octombrie pentru a vă asigura că aceste surse și destinații vor accepta conexiuni la și de la toate [adresele IP de EOP publicate](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5e69e-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="5e69e-107">Pentru mai multe informații despre această modificare, consultați postările din centrul de mesaje [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)sau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="5e69e-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="5e69e-108">**Notă**: dacă ați utilizat anterior publicarea IP sau URL prin intermediul actualizărilor HTML, XML și RSS pentru Endpoint, ar trebui, de asemenea, să migrați la noile servicii web pentru automatizarea acestor tipuri de actualizări.</span><span class="sxs-lookup"><span data-stu-id="5e69e-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="5e69e-109">Pentru mai multe informații, consultați [microsoft 365 Endpoint categorii și microsoft 365 IP Address și URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="5e69e-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
