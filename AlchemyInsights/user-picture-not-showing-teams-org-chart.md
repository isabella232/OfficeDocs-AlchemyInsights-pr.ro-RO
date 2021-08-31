---
title: Imaginea utilizatorului nu se afișează într-Microsoft Teams organizație
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792883"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Imaginea utilizatorului nu se afișează într-Microsoft Teams organizație

Dacă din organigramă lipsesc una sau mai multe persoane din organizația dvs., este posibil ca setarea **ShowInAddressLists** să fie setată la **False (Fals):**

1. Accesați Caseta Centru de administrare Microsoft 365 > [**utilizatori activi**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)și selectați utilizatorul cu fotografia lipsă. 
1. Selectați **fila Corespondență** și asigurați-vă **că Afișare în lista globală de adrese** este setată la **Da.** 

Dacă setarea **ShowInAddressLists** la **Da** nu funcționează, verificați următoarele:

- Este posibil ca utilizatorul să fie ascuns din lista de destinatari din Exchange. Pentru mai multe informații, consultați [Gestionarea listelor de adrese în Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Este posibil ca utilizatorul să fie ascuns din lista de adrese Azure Active Directory. Pentru mai multe informații, [consultați Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 
