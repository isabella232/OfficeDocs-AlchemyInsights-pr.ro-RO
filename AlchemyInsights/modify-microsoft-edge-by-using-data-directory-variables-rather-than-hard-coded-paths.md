---
title: Modificați Microsoft Edge utilizând variabile din directorul de date, mai degrabă decât căile codificate
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036854"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Modificați Microsoft Edge utilizând variabile din directorul de date, mai degrabă decât căile codificate

De exemplu, în Windows, pentru a stoca datele de profil sub datele aplicației locale ale unui utilizator, mai degrabă decât în locația implicită, setați politica *UserDataDir* la **$ {local_app_data} \Edge\Profile**.

Pentru mai multe informații, consultați [crearea de variabile pentru directorul de date utilizator Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).