---
title: Depanarea problemelor de grup
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714048"
---
# <a name="troubleshoot-group-issues"></a>Depanarea problemelor de grup

**Trebuie să atribui un grup unui rol de publicitate Azure**

Pentru a atribui un grup Azure Active Directory (AD) la un rol de publicitate Azure, efectuați pașii următori:

1. Creați un grup nou-pentru a crea un grup nou:

    un. Conectați-vă la centrul de administrare Azure AD cu administrator de rol privilegiat sau permisiuni de administrator global. 
    b. Selectați grupuri Azure Active Directory > > toate grupurile > grup nou. 
    c. Creați grupul.

2. Atribuiți rolul grupului fie în timpul creării grupului, fie după crearea grupului.

    un. Pentru a atribui un rol grupului în momentul creării unui grup, comutați la grupul se pot atribui rolurile de returnare Azure AD și puteți crea grupul.
    b. Pentru a atribui un rol grupului după ce a fost creat, navigați la fila roluri atribuite pentru grupul nou creat și atribuiți rolul grupului.

**Trebuie să gestionez apartenența la un grup atribuit la rolul Azure AD**

1. Pentru a împiedica elevația privilegiilor, în mod implicit, doar administratorul de rol privilegiat și administratorul global pot modifica apartenența la un grup atribuit unui rol. Cu toate acestea, pot alege să atribuie un proprietar unui astfel de grup și să delege această activitate. Pentru mai multe informații, consultați [utilizarea grupurilor Cloud pentru a gestiona atribuirile de roluri în Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Pentru întrebări frecvente și sfaturi de depanare pentru atribuirea rolurilor la grupuri din Azure AD, consultați [Depanarea rolurilor atribuite grupurilor Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Grupuri dinamice**

1. Dacă nu găsiți atributele de utilizator predefinite, asigurați-vă că atributul se află în lista de proprietăți acceptate.
2. În cazul în care căutați atributele dispozitivelor predefinite, asigurați-vă că atributul se află în lista de atribute de dispozitiv 
3. În plus față de atributele încorporate pentru utilizator și dispozitiv, puteți utiliza, de asemenea, [atributele de extensie](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). După sincronizarea atributelor de extensie din AD Windows Server local sau dintr-o aplicație SaaS conectată, atributele trebuie să fie vizibile în lista verticală a generatorului de reguli. Numele atributului particularizat poate fi găsit în director, dacă interogați atributul unui utilizator utilizând PowerShell și căutați numele atributului. Acestea pot fi utilizate și la construirea regulilor în sintaxa de regulă.
4. Asigurați-vă că entitatea găzduită are licența corespunzătoare. Grupurile dinamice impun entității găzduite să aibă o licență Azure AD P1 Premium. Lista de planuri de licență Azure AD poate fi accesată [aici](https://azure.microsoft.com/pricing/details/active-directory/). Planurile de licențiere Enterprise Mobility + pot fi accesate [aici](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Asigurați-vă că rolul utilizatorului care creează grupul dinamic este un administrator global, un administrator Intune, un administrator de grup sau un administrator de utilizator.
6. Vă rugăm să permiteți timpul ca grupul să fie populat. În funcție de dimensiunea entității găzduite, grupul poate dura până la 24 de ore pentru populare pentru prima dată sau după o modificare de regulă.
7. Pentru mai multe informații, consultați [crearea regulilor bazate pe atribute pentru apartenența dinamică la grup](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Trebuie să șterg un grup**

1. Grupurile pot fi șterse din Director utilizând cmdletul Remove-AzureADGroup din modulul Azure AD PowerShell.
2. Înainte de a încerca să ștergeți un grup sincronizat din Azure AD, asigurați-vă că ați șters toate licențele atribuite pentru a evita erorile.
3. Pentru mai multe informații despre ștergerea grupurilor, consultați [ștergerea unui grup cu o licență atribuită](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Trebuie să restaurez un grup șters**

1. Dacă un grup Office 365 este șters, acesta poate fi restaurat doar cu până la 30 de zile înainte de a avea loc ștergerea permanentă. După ce ați șters definitiv, grupul nu mai poate fi restaurat. Aflați mai multe despre restaurarea grupurilor [aici](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Această funcționalitate nu este acceptată pentru grupurile de securitate și grupurile de distribuire.
3. Asigurați-vă că sunteți autorizat să restaurați un grup Office 365. Administratorii globali, administratorii de grup, administratorii contului de utilizator, administratorii de servicii Intune, asistența pentru parteneri Tier1 sau Tier2 și proprietarul grupului poate restaura un grup.
4. Atunci când un grup dinamic este șters și restaurat, acesta este văzut ca un grup nou și repopulat conform regulii. Acest proces poate dura până la 24 de ore.
5. Pentru mai multe informații despre restaurarea unui grup șters, consultați [restaurarea unui grup Office 365 șters din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Configurarea politicii de expirare a grupurilor**

1. Această funcționalitate este acceptată doar pentru grupurile Office 365 și nu pentru grupurile de securitate și grupurile de distribuire nu sunt acceptate.
2. Configurarea și utilizarea politicii de expirare pentru grupurile Office 365 necesită o licență Azure AD Premium.
3. În prezent, se poate configura o singură politică de expirare pentru grupurile Office 365 pentru o entitate găzduită.
4. Doar administratorii globali, administratorii de grup, administratorii de utilizator și proprietarul grupului pot reînnoi un grup.
5. Dacă un grup Office 365 este expirat, acesta este șters și poate fi restaurat doar cu până la 30 de zile înainte de a avea loc ștergerea permanentă. După ce ați șters definitiv, grupul nu mai poate fi restaurat. Aflați mai multe despre restaurarea grupurilor [aici](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Reînnoirea automată bazată pe activitate**

Activitățile de utilizator din SharePoint, Outlook și teams pot declanșa reînnoirea automată a grupului. Activitățile sunt verificate la 35 de zile înainte de expirarea unui grup. Dacă există activitate în timpul ciclului de viață al grupului curent, grupul va fi reînnoit automat și notificarea prin e-mail nu va fi trimisă proprietarilor de grup.

**Temporizarea notificării pentru grupurile expirate**

1. Notificările prin e-mail sunt trimise proprietarilor de grup Office 365 30 de zile, 15 zile și 1 zi înainte de expirarea grupului.
2. Atunci când configurați pentru prima dată expirarea, toate grupurile mai vechi decât intervalul de expirare sunt setate la 35 zile până la expirare.
3. Data de expirare a grupului este calculată pe baza datei de reînnoire a grupului, nu pe baza datei actualizate a politicii. Dacă Politica de expirare este actualizată, data de expirare nu se va modifica.
4. Pentru mai multe informații, consultați [Politica de expirare a grupurilor și e-mailurile de reînnoire](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) și [restaurarea unui grup Office 365 șters în Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Permisiunea de a crea un grup**

Asigurați-vă că sunteți autorizat să creați un grup nou. Administratorii globali pot dezactiva crearea grupurilor în portalul Azure sau în panoul de acces. Este posibil să aveți nevoie de un administrator pentru a crea noul grup sau pentru a vă oferi permisiuni corespunzătoare.

1. [Crearea unui grup nou și adăugarea de membri în portalul Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Crearea grupurilor în PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Dezactivarea creării grupurilor în PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Gestionarea persoanelor care pot crea grupuri în Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Dezactivarea notificării de bun venit Office 365 prin PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Rolurile administrative Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Gestionarea permisiunilor de creare a grupurilor**

1. Administratorii globali pot gestiona permisiunile de creare a grupurilor pentru grupurile de securitate sau Office 365 create în portalul Azure sau în panoul de acces, setând **utilizatorii pot crea grupuri de securitate în portaluri Azure** sau **utilizatorii pot crea grupuri Office 365 în setările Azure portaluri** din **toate grupurile > general (Setări)**.
2. De asemenea, puteți restricționa crearea grupurilor pentru a selecta un grup de utilizatori dacă aveți o licență Azure AD P1 Premium.

**Dezactivarea notificării de bun venit pentru noii membri ai unui grup Office 365**

Notificarea de bun venit trimisă utilizatorilor care sunt adăugați la Office 365 Groups poate fi dezactivată prin setarea `UnifiedGroupWelcomeMessageEnabled` la **false** în PowerShell. Aflați mai multe despre această setare [aici](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













