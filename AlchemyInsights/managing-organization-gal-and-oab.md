---
title: Gestionarea listei globale de adrese de organizație și a agendei offline
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794844"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="33cba-102">Gestionarea listei globale de adrese de organizație (GAL) și a agendei offline (OAB)</span><span class="sxs-lookup"><span data-stu-id="33cba-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="33cba-103">O listă globală de adrese (GAL) este o listă de obiecte activate pentru e-mail (orice tip de destinatar care poate primi e-mail) în cadrul organizației.</span><span class="sxs-lookup"><span data-stu-id="33cba-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="33cba-104">În fiecare organizație este creată automat o singură GAL.</span><span class="sxs-lookup"><span data-stu-id="33cba-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="33cba-105">Puteți crea GAL-uri suplimentare pentru a separa utilizatorii după organizație sau locație, dar un utilizator poate vedea și utiliza o singură GAL odată.</span><span class="sxs-lookup"><span data-stu-id="33cba-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="33cba-106">Unii clienți de e-mail, cum ar fi Outlook pentru Windows, descarcă GAL pentru utilizare offline.</span><span class="sxs-lookup"><span data-stu-id="33cba-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="33cba-107">Această operație este cunoscută sub numele de agendă offline (OAB).</span><span class="sxs-lookup"><span data-stu-id="33cba-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="33cba-108">În Exchange Online, o OAB este actualizată o dată la 8 ore, după care clienții trebuie să o descarce pentru a actualiza copia locală OAB.</span><span class="sxs-lookup"><span data-stu-id="33cba-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="33cba-109">Orice modificare a destinatarului trebuie să fie vizibilă mai întâi în GAL, iar mai târziu în OAB.</span><span class="sxs-lookup"><span data-stu-id="33cba-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="33cba-110">Iată câteva proceduri GAL și OAB utilizate frecvent:</span><span class="sxs-lookup"><span data-stu-id="33cba-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="33cba-111">Din mai multe motive, veți prefera ca unele obiecte să fie ascunse din GAL.</span><span class="sxs-lookup"><span data-stu-id="33cba-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="33cba-112">Consultați [Ascundeți destinatarii din listele de adrese](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="33cba-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="33cba-113">Dacă trebuie să le oferiți unor grupuri de utilizatori vizualizări particularizate ale GAL-ului organizației, consultați [Politicile de agendă din Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="33cba-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="33cba-114">[Creați o listă globală de adrese în Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), iar pentru a afla cum să lucrați cu permisiunile GAL, consultați [Liste de adrese în Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="33cba-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="33cba-115">Rețineți că, dacă creați GAL-uri noi, ar trebui să creați și o nouă OAB.</span><span class="sxs-lookup"><span data-stu-id="33cba-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="33cba-116">Consultați [Proceduri privind Agenda offline](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="33cba-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
