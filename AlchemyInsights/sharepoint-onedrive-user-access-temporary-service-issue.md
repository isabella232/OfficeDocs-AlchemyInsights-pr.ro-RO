---
title: Probleme de performanță-SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771256"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint sau OneDrive este lent, inaccesibil sau indisponibil pentru mai mulți utilizatori

Dacă un site OneDrive sau SharePoint nu este disponibil pentru mai mulți utilizatori care au avut acces anterior, este posibil să existe o problemă de serviciu temporară. [Verificați tabloul de bord pentru starea serviciilor](https://portal.office.com/adminportal/home#/servicehealth).

**Adăugarea și licența utilizatorului**

Asigurați-vă că [atribuiți licențe utilizatorilor din Microsoft 365 pentru Business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Atribuirea permisiunilor**

Dacă utilizatorului i s-a atribuit o licență SharePoint și încă primește un mesaj de acces refuzat, asigurați-vă că au atribuit [nivelul de permisiune corespunzător](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Luați în considerare utilizarea caracteristicii de solicitare de acces**

[Caracteristica de solicitare de acces](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite persoanelor să solicite acces la conținut pe care nu le pot vedea momentan.

**Permiteți ca scriptul particularizat să provoace probleme de acces refuzat**

Există anumite scenarii în care *opțiunea se permite script particularizat* să prezinte un acces refuzat. Pentru o listă de caracteristici afectate, considerații de securitate și capacitatea de a dezactiva caracteristica. Vă rugăm să vizitați [Permiteți sau să împiedicați scriptul particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

