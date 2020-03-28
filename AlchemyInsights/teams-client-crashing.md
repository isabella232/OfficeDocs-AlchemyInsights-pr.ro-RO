---
title: Clientul Teams are căderi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030676"
---
# <a name="teams-client-crashing"></a>Clientul Teams are căderi?

Dacă clientul dvs. Teams are căderi, încercați următoarele:

- Dacă utilizați aplicația desktop Teams, [asigurați-vă că aplicația este complet actualizată](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Asigurați-vă că toate [URL-urile și intervalele de adrese Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) sunt accesibile.

- Conectați-vă cu contul dvs. de administrator și verificați [Tabloul de bord cu starea serviciilor](https://docs.microsoft.com/office365/enterprise/view-service-health) pentru a verifica dacă există vreo întrerupere sau degradare a serviciului.

 - Ca ultim pas, puteți încerca să goliți memoria cache a clientului Teams:

    1.  Ieșiți complet din clientul desktop Microsoft Teams. Puteți să faceți dreapta pe **Teams** din bara de pictograme, apoi să faceți clic pe **Ieșire** sau să rulați Manager de activități și să anihilați complet procesul.

    2.  Mergeți la Explorer și tastați %appdata%\Microsoft\teams.

    3.  Când vă aflați în director, veți vedea câteva dintre următoarele foldere:

         - Din **Application Cache**, accesați Cache și ștergeți orice fișier din locația de cache: %appdata%\Microsoft\teams\application cache\cache.

        - Din **Blob_storage**, ștergeți toate fișierele: %appdata%\Microsoft\teams\blob_storage.

        - Din **Cache**, ștergeți toate fișierele: %appdata%\Microsoft\teams\Cache.

        - Din **databases**, ștergeți toate fișierele: %appdata%\Microsoft\teams\databases.

        - Din **GPUCache**, ștergeți toate fișierele: %appdata%\Microsoft\teams\GPUcache.

        - Din **IndexedDB**, ștergeți fișierul .db: %appdata%\Microsoft\teams\IndexedDB.

        - Din **Local Storage**, ștergeți toate fișierele: %appdata%\Microsoft\teams\Local Storage.

        - În final, din **tmp**, ștergeți orice fișier: %appdata%\Microsoft\teams\tmp.

    4. Reporniți clientul Teams.
