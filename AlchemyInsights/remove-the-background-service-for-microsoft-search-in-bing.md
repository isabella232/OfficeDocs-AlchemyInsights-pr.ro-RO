---
title: Eliminarea serviciului de fundal pentru Microsoft Search în Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816335"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Eliminarea serviciului de fundal pentru Microsoft Search în Bing

Pentru a elimina serviciul de fundal pentru Microsoft Search în Bing, puteți încerca următoarele căi de atac:

1. Pentru a reveni la setările motorului de căutare inițial, procedați astfel:

    un. Comutați opțiunea **Utilizați Bing ca motor de [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) căutare implicit dezactivat**.

    b. [Accesați centrul de administrare Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) și debifați setarea care afectează toți utilizatorii din organizația dvs.

2. Pentru a elimina serviciul de fundal de pe un dispozitiv individual, procedați astfel:

    un. Alegeți **Panou de Control > programe > programe și caracteristici**.

    b. Faceți clic cu butonul din dreapta pe **Microsoft Search în Bing** sub lista de programe instalate, apoi faceți clic pe **Dezinstalare**.

3. Pentru a elimina serviciul de fundal de pe mai multe dispozitive din organizație, conectați-vă ca administrator și derulează următoarea comandă într-un script: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
