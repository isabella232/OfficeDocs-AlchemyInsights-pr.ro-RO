---
title: Depanarea problemelor audio în Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796315"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="f69be-102">Depanarea problemelor audio în Windows 10</span><span class="sxs-lookup"><span data-stu-id="f69be-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="f69be-103">**Rulați depanatorul audio**</span><span class="sxs-lookup"><span data-stu-id="f69be-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="f69be-104">Este posibil ca depanatorul audio să poată remedia automat problemele audio:</span><span class="sxs-lookup"><span data-stu-id="f69be-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="f69be-105">Selectați **Start**, tastați **Depanare**, apoi selectați **Depanare** din lista de rezultate.</span><span class="sxs-lookup"><span data-stu-id="f69be-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="f69be-106">Selectați **redarea audio** > **Rulați depanatorul**.</span><span class="sxs-lookup"><span data-stu-id="f69be-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="f69be-107">**Verificați cablurile, volumul, boxele și căștile**</span><span class="sxs-lookup"><span data-stu-id="f69be-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="f69be-108">Verificați conexiunile difuzoarelor și ale căștilor pentru cabluri libere și asigurați-vă că sunt conectate la mufa corectă.</span><span class="sxs-lookup"><span data-stu-id="f69be-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="f69be-109">Verificați nivelul de putere și volum și încercați să răsuci toate controalele de volum în sus.</span><span class="sxs-lookup"><span data-stu-id="f69be-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="f69be-110">Unele difuzoare și aplicații au propriile lor controale de volum și s-ar putea să trebuiască să le verificați pe toate pentru a vă asigura că sunt la nivelurile corecte.</span><span class="sxs-lookup"><span data-stu-id="f69be-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="f69be-111">Încercați să vă conectați utilizând un alt port USB.</span><span class="sxs-lookup"><span data-stu-id="f69be-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="f69be-112">**Notă:** Rețineți că este posibil ca difuzoarele să nu funcționeze atunci când sunt conectate căști.</span><span class="sxs-lookup"><span data-stu-id="f69be-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="f69be-113">**Verificare Manager dispozitive**</span><span class="sxs-lookup"><span data-stu-id="f69be-113">**Check Device Manager**</span></span>

<span data-ttu-id="f69be-114">Pentru a vă asigura că driverele sunt actualizate:</span><span class="sxs-lookup"><span data-stu-id="f69be-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="f69be-115">Selectați **Start**, tastați **Manager dispozitive**, apoi selectați **Manager dispozitive** din lista de rezultate.</span><span class="sxs-lookup"><span data-stu-id="f69be-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="f69be-116">Sub **Controlere de sunet, video și jocuri**, selectați placa de sunet, deschideți-o, selectați fila **driver** și selectați **Actualizare driver**.</span><span class="sxs-lookup"><span data-stu-id="f69be-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="f69be-117">**Notă:** Dacă Windows nu găsește un driver nou, căutați unul pe site-ul web al producătorului dispozitivului și urmați instrucțiunile lor.</span><span class="sxs-lookup"><span data-stu-id="f69be-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="f69be-118">**Reinstalați driverul**</span><span class="sxs-lookup"><span data-stu-id="f69be-118">**Reinstall the driver**</span></span>

<span data-ttu-id="f69be-119">Dacă nu puteți să actualizați prin Device Manager sau să găsiți un driver nou pe site-ul web al producătorului, încercați acești pași:</span><span class="sxs-lookup"><span data-stu-id="f69be-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="f69be-120">În Device Manager, faceți clic dreapta (sau apăsați lung) pe driverul audio și selectați **Dezinstalare**.</span><span class="sxs-lookup"><span data-stu-id="f69be-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="f69be-121">Reporniți dispozitivul și Windows va încerca să reinstaleze driverul.</span><span class="sxs-lookup"><span data-stu-id="f69be-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="f69be-122">Dacă reinstalarea driverului nu funcționează, încercați să utilizați driverul audio generic care vine cu Windows.</span><span class="sxs-lookup"><span data-stu-id="f69be-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="f69be-123">În Device Manager, faceți clic dreapta (sau apăsați continuu) driverul audio > **Actualizare software** > de driver > **Răsfoiți computerul meu pentru software de driver\*\*\*\*Permiteți-mi să aleg dintr-o listă de drivere de dispozitiv de pe computerul meu**, selectați **dispozitiv audio de înaltă definiție**, selectați **Următorul**și urmați instrucțiunile pentru a-l instala.</span><span class="sxs-lookup"><span data-stu-id="f69be-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="f69be-124">**Setarea dispozitivului implicit**</span><span class="sxs-lookup"><span data-stu-id="f69be-124">**Set the default device**</span></span>

<span data-ttu-id="f69be-125">Dacă vă conectați la un dispozitiv audio utilizând USB sau HDMI, este posibil să fie necesar să setați dispozitivul respectiv ca implicit:</span><span class="sxs-lookup"><span data-stu-id="f69be-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="f69be-126">Selectați **Start**, tastați **sunet**, apoi selectați sunete **sau** **modificați sunetele sistemului** din lista de rezultate.</span><span class="sxs-lookup"><span data-stu-id="f69be-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="f69be-127">În fila **Redare** , selectați un dispozitiv, selectați **Setați implicit**, apoi selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="f69be-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

