---
title: Modificarea Microsoft Edge utilizând variabile de director de date, mai degrabă decât căi codificate
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113428"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Modificarea Microsoft Edge utilizând variabile de director de date, mai degrabă decât căi codificate

De exemplu, pe Windows, pentru a stoca datele de profil sub datele de aplicație locale ale unui utilizator, nu în locația implicită, setați politica **UserDataDir** la **${local_app_data}\Edge\Profile.** 

Pentru a afla mai multe, [consultați Crearea Microsoft Edge variabile ale directorului de date de utilizator.](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)