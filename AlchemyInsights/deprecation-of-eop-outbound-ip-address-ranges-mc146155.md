---
title: 1065 Dezaprobarea intervalelor de adrese IP de ieșire EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704609"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="0137b-102">Dezaprobarea intervalelor de adrese IP de ieșire ale EOP</span><span class="sxs-lookup"><span data-stu-id="0137b-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="0137b-103">Am detectat o problemă potențială cu organizația dvs., care (dacă nu este corectată până la 26 octombrie 2018) ar putea întrerupe fluxul de corespondență către destinațiile locale sau externe.</span><span class="sxs-lookup"><span data-stu-id="0137b-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="0137b-104">După s-a comunicat anterior, pentru a simplifica gestionarea intervalului de adrese IP, consolidăm intervalele de adrese IP Exchange Online Protection (EOP) care sunt utilizate pentru a trimite și primi e-mailuri în afara Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0137b-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="0137b-105">Analiza noastră indică faptul că una sau mai multe surse de e-mail externe sau destinații pe care le-ați configurat în conectorii fluxului de corespondență nu acceptă conexiuni din intervalele de adrese IP afișate [aici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0137b-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="0137b-106">Acționați înainte de 26 octombrie pentru a vă asigura că aceste surse și destinații vor accepta conexiuni la și de la toate [adresele IP EOP publicate](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0137b-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="0137b-107">Pentru mai multe informații despre această modificare, vă rugăm să consultați Mesaje Center posturi [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)sau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="0137b-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="0137b-108">**Notă:** Dacă ați utilizat anterior publicarea IP sau URL prin HTML, XML și RSS pentru actualizări de puncte finale, de asemenea, ar trebui să migreze la noile servicii web pentru automatizarea acestor tipuri de actualizări.</span><span class="sxs-lookup"><span data-stu-id="0137b-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="0137b-109">Pentru mai multe informații, consultați [Categoriile de puncte finale Microsoft 365 și serviciul web Microsoft 365 IP Address and URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="0137b-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
