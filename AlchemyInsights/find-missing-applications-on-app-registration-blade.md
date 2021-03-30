---
title: Găsirea aplicațiilor lipsă în blade de înregistrare a aplicațiilor
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405218"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Găsirea aplicațiilor lipsă în blade de înregistrare a aplicațiilor

1. Nu găsiți aplicații în portalul de înregistrare a aplicațiilor.

    Dacă o aplicație este o aplicație cu mai multe entități găzduite și a fost înregistrată în altă entitate găzduită, aceasta nu se va afișa sub Blade de înregistrare a aplicațiilor. Totuși, o puteți găsi sub Enterprise Applications blade după ce aceasta a fost accesată (după consimțământul dvs.) și entitatea principală de serviciu a fost creată în entitatea găzduită. Pentru mai multe informații, [consultați Aplicațiile & principale de serviciu din Azure AD - platforma de identitate Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Nu puteți să vizualizați aplicații în blade de înregistrare a aplicațiilor chiar dacă sunteți administrator.

    Asigurați-vă că sunteți în directorul potrivit pe portalul Azure.
3. Aplicația mea nu este listată sub blade pentru aplicații enterprise, dar apare atunci când interogăm comanda PowerShell.

    Uneori, după ce ștergeți aplicația din portalul Azure, aceasta nu se afișează în portal, dar este posibil să nu fi fost ștearsă complet. Pentru mai multe informații, consultați:
    - Puteți să regăsiți lista de aplicații șterse anterior și să vedeți dacă aplicația apare în listă utilizând comanda Powershell: **Get-AzureADDeletedApplication**. Pentru a afla mai multe, [consultați Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Dacă doriți să eliminați complet aplicația, puteți încerca următoarele în PowerShell: **Remove-AzureADApplication -ObjectId**. Pentru a afla mai multe, [consultați Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Alternativ, puteți încerca să restaurați aplicația ștearsă utilizând următoarea comandă Powershell: **Restore AzureADDeletedApplication -ObjectId**. Pentru a afla mai multe, [consultați Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Nu pot găsi lista cu toate aplicațiile enterprise preinstalate în noua mea entitate găzduită Azure.

    Nu există aplicații de întreprindere preinstalate în Azure AD în mod implicit. Trebuie să o adăugați manual din opțiunea "Aplicație nouă" răsfoind-o din galeria Azure AD sau adăugați o aplicație non-galerie. Pentru a afla mai multe, [consultați Pornire rapidă: Adăugarea unei aplicații la entitatea găzduită Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Dacă sunteți administrator global, vă puteți accesa cu ușurință aplicațiile utilizând [Lansatorul de aplicații Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Nu îmi pot găsi aplicațiile din portalul Aplicațiile mele.

    Asigurați-vă că nu sunt ascunse aplicațiile din pagina colecției Aplicațiile mele. Pentru a afla mai multe, [consultați Colecții (previzualizare) în portalul Aplicațiile mele - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Pentru a porni aplicații din portalul Aplicațiile mele, consultați [Găsirea aplicațiilor & pe portalul Aplicațiile mele - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Aplicația Office 365 Mover nu se afișează pe enterprise Applications blade după instalare.

    Aplicația "Office 365 Mover" este o aplicație pentru mai multe imprimante care nu trebuie adăugată la AAD utilizând secțiunea Galerie aplicații de sub Înregistrare aplicații Enterprise. Pentru a accesa aplicația Office 365 Mover, pur și simplu conectați-vă la aplicație și solicitați consimțământul utilizatorului pentru permisiuni. După ce utilizatorul oferă consimțământul, această aplicație va fi adăugată automat la entitatea găzduită cu ID-ul de e-mail pe care l-ați conectat.

    După ce vă conectați la aplicație, ar trebui să puteți găsi intrarea acestei aplicații sub sistemul blade Enterprise Applications din AAD. Trebuie să căutați aplicația fie tastând numele complet, adică "Office 365 Mover", fie pur și simplu căutați "office" și ar trebui să listze aplicația. Pentru a afla mai multe, consultați [Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)spune că este deja instalat, dar nu este listat în galeria Aplicații enterprise.
8. Pornire rapidă: Vizualizați lista de aplicații care utilizează entitatea găzduită [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) pentru gestionarea identităților vă arată cum să vizualizați aplicațiile, cunoscute și ca aplicații, care sunt configurate deja să utilizeze entitatea găzduită Azure AD ca furnizor de identitate (IDP).
9. [Depanați problema obișnuită cu adăugarea sau](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) eliminarea unei aplicații în Azure Active Directory vă ajută să înțelegeți problemele comune cu vizualizarea aplicațiilor în Azure Active Directory.
