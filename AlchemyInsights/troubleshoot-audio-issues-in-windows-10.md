---
title: Depanarea problemelor audio în Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750325"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Depanarea problemelor audio în Windows 10

**Rularea depanatorului audio**

1.  Deschideți [setările de depanare](ms-settings:troubleshoot).

2.  Selectați **Redare audio**  >  **Rulați depanatorul**.

**Setarea dispozitivului implicit**

Dacă vă conectați la un dispozitiv audio utilizând USB sau HDMI, poate fi necesar să setați acel dispozitiv ca implicit:

1. Deschideți **pornire**  >  **sunet**, apoi selectați **sunet** sau **modificare sunete de sistem** din lista de rezultate.

2.  Pe fila **Redare** , selectați un dispozitiv, selectați **Setare implicit**, apoi selectați **OK**.

**Verificați cablurile, volumul, difuzoarele și căștile**

1. Verificați conexiunile difuzoarelor și ale căștilor pentru cablurile libere și asigurați-vă că sunt conectate la mufa corectă.

2. Verificați nivelurile puterii și volumului și încercați să transformați toate controalele de volum în sus.

3. Unele difuzoare și aplicații au propriile controale de volum; poate fi necesar să le verificați pe toate pentru a vă asigura că acestea sunt la nivelurile corecte.

4. Încercați să vă conectați utilizând un alt port USB.

**Notă: rețineți**că este posibil ca difuzoarele să nu funcționeze atunci când sunt conectate căști.

**Verificați Manager dispozitive**

Pentru a vă asigura că driverele sunt la zi:

1. Selectați **Start**, tastați **Manager dispozitive**, apoi selectați **Manager dispozitive** din lista de rezultate.

2. Sub **Controlere de sunet, video și jocuri**, selectați placa de sunet, deschideți-o, selectați fila **driver** și selectați **Actualizare driver**.

**Notă**: dacă Windows nu găsește un driver nou, căutați unul pe site-ul web al producătorului dispozitivului și urmați instrucțiunile.

**Reinstalați driverul**

Dacă nu puteți să actualizați prin Device Manager sau să găsiți un driver nou pe site-ul web al producătorului, încercați acești pași:

1. În Manager dispozitive, faceți clic dreapta (sau apăsați lung) pe driverul audio și selectați **Dezinstalare**. Reporniți dispozitivul și Windows va încerca să reinstaleze driverul.

2. Dacă reinstalarea driverului nu funcționează, încercați să utilizați driverul audio generic livrat cu Windows. În Manager dispozitive, faceți clic dreapta (sau apăsați lung) driverul audio > **Actualizare software**  >  **de driver răsfoiți computerul meu pentru software de driver**  >  **Permiteți-mi să aleg dintr-o listă de drivere de dispozitiv de pe computer**, selectați **dispozitiv audio de înaltă definiție**, selectați **Următorul**și urmați instrucțiunile pentru a-l instala.
