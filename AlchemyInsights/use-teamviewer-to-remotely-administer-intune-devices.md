---
title: Utilizarea TeamViewer pentru administrarea de la distanță a dispozitivelor Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555246"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="4b0ad-102">Utilizarea TeamViewer pentru administrarea de la distanță a dispozitivelor Intune</span><span class="sxs-lookup"><span data-stu-id="4b0ad-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="4b0ad-103">Dispozitivele gestionate de Intune pot fi administrate de la distanță utilizând [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="4b0ad-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="4b0ad-104">Pentru a administra Intune utilizând TeamViewer, utilizați acești pași:</span><span class="sxs-lookup"><span data-stu-id="4b0ad-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="4b0ad-105">Începeți prin a obține acreditări de la TeamViewer pentru a configura Conectorul TeamViewer pe Intune.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="4b0ad-106">Acest lucru permite administratorului să introducă acreditări în interfața de utilizator a conectorului TeamViewer sub Dispozitive, o operațiune o singură dată pentru a stabili legătura dintre Intune și serviciul TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="4b0ad-107">**Partea 1: Începerea unei sesiuni cu un dispozitiv la distanță**</span><span class="sxs-lookup"><span data-stu-id="4b0ad-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="4b0ad-108">Sub **Toate dispozitivele**, selectați dispozitivul cu care doriți să începeți o sesiune la distanță.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="4b0ad-109">De la **... Mai mult**, selectați **Sesiune nouă de asistență la distanță**.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="4b0ad-110">Selectați **Da** pentru a confirma că doriți să stabiliți o sesiune la distanță.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="4b0ad-111">După ce solicitarea "Inițierea unei noi sesiuni la distanță" este recunoscută de serviciul TeamViewer, veți vedea o opțiune pentru **a porni asistența la distanță** sub detaliile panoului Prezentare generală (sau, Essentials) pentru dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="4b0ad-112">Selectați **Vedeți mai multe** pentru a extinde panoul și a afișa starea Asistență la distanță.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="4b0ad-113">Selectați **Pornire sesiune la distanță** pentru a iniția sesiunea pe partea de administrator.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="4b0ad-114">Alegeți să descărcați binarul TeamViewer (Windows) și selectați **Executare**.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="4b0ad-115">**Notă** Puteți ignora orice pagină de browser web deschisă site-ului Web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="4b0ad-116">Confirmați solicitarea ca aplicația TeamViewer să efectueze modificări pe dispozitiv (numai Windows).</span><span class="sxs-lookup"><span data-stu-id="4b0ad-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="4b0ad-117">Aplicația TeamViewer pornește și include codul de sesiune pentru a autentifica conexiunea cu dispozitivul la distanță.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="4b0ad-118">**Partea 2: Pe dispozitivul vizat pentru o sesiune la distanță**</span><span class="sxs-lookup"><span data-stu-id="4b0ad-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="4b0ad-119">Deschideți portalul companiei Intune.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="4b0ad-120">Căutați un semnalizator de notificare: "Administratorul IT solicită controlul acestui dispozitiv pentru o sesiune de asistență la distanță" și selectați notificarea.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="4b0ad-121">Alegeți să descărcați aplicația TeamViewer sau să confirmați descărcarea aplicației TeamViewer din magazinul de aplicații și selectați **Executare**.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="4b0ad-122">**Notă** Puteți ignora orice pagină de browser web deschisă site-ului Web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="4b0ad-123">Confirmați solicitarea ca aplicația TeamViewer să efectueze modificări pe dispozitiv (numai Windows).</span><span class="sxs-lookup"><span data-stu-id="4b0ad-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="4b0ad-124">Aplicația TeamViewer pornește și include codul de sesiune pentru a autentifica conexiunea cu dispozitivul la distanță.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="4b0ad-125">Un pop-up întreabă dacă doriți să permiteți începerea sesiunii.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="4b0ad-126">**Notă** Codurile de sesiune generate de serviciul TeamViewer sunt utilizate o singură dată.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="4b0ad-127">Dacă pierdeți conexiunea, trebuie:</span><span class="sxs-lookup"><span data-stu-id="4b0ad-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="4b0ad-128">Închideți instanța aplicației TeamViewer pe dispozitivul la distanță și pe aplicația de lucru de administrare.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="4b0ad-129">Închideți portalul companiei pe dispozitivul la distanță.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="4b0ad-130">Inițiați o nouă "Sesiune nouă de asistență la distanță" din portalul de administrare.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="4b0ad-131">Redeschideți portalul companiei pe dispozitivul la distanță pentru a primi noua notificare.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="4b0ad-132">Descărcați și deschideți aplicația TeamViewer atât pe dispozitivul la distanță, cât și pe aplicația de lucru de administrare, ca și până acum.</span><span class="sxs-lookup"><span data-stu-id="4b0ad-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>