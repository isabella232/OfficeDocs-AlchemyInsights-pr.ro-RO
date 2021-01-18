---
title: Problemă la asocierea la VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885664"
---
# <a name="issue-joining-vms"></a>Problemă la asocierea la VMs

Pentru a rezolva problemele care apar când încercați să vă asociați la VMs, efectuați pașii următori:

1. Încercați să vă conectați utilizând formatul **UPN** (de exemplu, "JoeUser@contoso.com") în loc de formatul **sAMAccountName** (' CONTOSO\joeuser ').
2. Asigurați-vă că ați activat sincronizarea parolei în conformitate cu pașii schițați *în Ghidul introductiv* .
3. Asigurați-vă că contul de utilizator afectat nu este un cont extern în entitatea găzduită Azure AD. Utilizatorii externi nu se pot conecta la domeniul gestionat deoarece serviciile de domeniu Azure AD nu au acreditări pentru astfel de conturi de utilizator.
4. Dacă contul de utilizator afectat este un cont de utilizator în cloud, asigurați-vă că utilizatorii și-au schimbat parola după ce ați activat serviciile de domeniu Azure AD. Acest pas determină hash-ul de acreditări necesar pentru ca serviciile de domeniu Azure AD să fie generate.
5. Dacă conturile de utilizator afectate sunt sincronizate dintr-un director local, Verificați dacă a fost configurată versiunea recomandată de Azure AD Connect pentru a efectua o sincronizare completă.
6. Dacă problemele persistă după ce confirmați pasul 4, efectuați următoarele comenzi de la mașina de sincronizare:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.