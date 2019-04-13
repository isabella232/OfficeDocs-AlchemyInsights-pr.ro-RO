---
title: 1065 dezaprobare EOP outbound IP adresa rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858108"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="15840-102">Dezaprobare de EOP ieşire variază de adresa IP</span><span class="sxs-lookup"><span data-stu-id="15840-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="15840-103">Ne-am detectat o problemă potenţială cu organizaţiei (dacă nu este corectată de 26 octombrie 2018) s-ar putea rupe fluxul de corespondenţă de la local sau destinaţii externe.</span><span class="sxs-lookup"><span data-stu-id="15840-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="15840-104">Ca anterior comunicate, pentru a simplifica gestionarea gama IP adresa, am centralizaţi Exchange Online protecţia (EOP) IP adresa intervalele care sunt folosite pentru a trimite şi primi poştă electronică în afara de Office 365.</span><span class="sxs-lookup"><span data-stu-id="15840-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="15840-105">Analiza noastră indică faptul că una sau mai multe de e-mail extern surse sau destinaţii care aţi configurat în conectorii de fluxul de corespondenţă nu sunt accepta conexiuni de la IP adresă intervalele afişate [aici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="15840-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="15840-106">Acţionează înainte de 26 octombrie, pentru a asigura aceste surse şi destinaţii va accepta conexiuni la şi de la toate [adresele EOP IP a publicat](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="15840-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="15840-107">Pentru mai multe informaţii despre această schimbare, vă rugăm să consultaţi Centrul de mesaje posturi [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)sau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="15840-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="15840-108">**Notă**: dacă aţi utilizat anterior publicarii IP sau URL-ul prin intermediul HTML, XML şi RSS pentru actualizări de final, de asemenea, ar trebui să migra la noile servicii web pentru automatizarea acestor tipuri de actualizări.</span><span class="sxs-lookup"><span data-stu-id="15840-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="15840-109">Pentru mai multe informaţii, a se vedea [categoriile de endpoint Office 365 si Office 365 adresa IP şi URL serviciu web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="15840-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
