---
title: Imaginea de utilizator apare încă în Microsoft Teams organizație
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422321"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Imaginea de utilizator apare încă în Microsoft Teams organizație

Dacă una sau mai multe persoane din organizația dvs. au fost dezactivate sau eliminate, iar fotografia lor de profil apare încă în organigramă, este posibil ca setarea **ShowInAddressLists** să fie setată la False (Fals): 

1. Accesați Caseta Centru de administrare Microsoft 365 > [Utilizatori activi și](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) selectați utilizatorul cu fotografia care încă apare. 
1. Selectați **fila Corespondență** și asigurați-vă **că Afișare în lista globală de** adrese este setată la **Nu.**

Dacă setarea **ShowInAddressLists** la **Nu** nu funcționează, verificați următoarele: 

- Este posibil ca utilizatorul să fie afișat din lista de destinatari în Exchange. Pentru mai multe informații, consultați [Gestionarea listelor de adrese Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Este posibil ca utilizatorul să fie afișat din lista de adrese din Azure Active Directory. Pentru mai multe informații, [consultați Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 