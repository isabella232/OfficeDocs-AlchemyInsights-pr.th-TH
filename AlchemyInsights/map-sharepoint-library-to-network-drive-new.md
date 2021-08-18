---
title: แมปSharePointไปยังไดรฟ์เครือข่าย
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 741d22c4231886b385b0bc2361e429929ef58f4b84d56e51186f129fc5d07921
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57901607"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>แมปSharePointไปยังไดรฟ์เครือข่าย

แทนที่จะแมปไดรฟ์เครือข่าย SharePointไฟล์ด้วยไคลเอ็นต์ การซิงค์สําหรับ OneDriveใหม่ ซึ่งมีการเข้าถึงไฟล์ได้ตามต้องการ เข้าถึงไฟล์ของคุณทั้งหมดใน OneDriveโดยไม่ต้องใช้พื้นที่จัดเก็บข้อมูลภายในเครื่อง For more information, see [Sync SharePoint Teams files with your computer](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) and Save disk space with OneDrive Files [On-Demand for Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).

ถ้าคุณเลือกแมปไดรฟ์แทนการใช้ไคลเอ็นต์ การซิงค์สําหรับ OneDrive[ตรวจสอบ](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)ให้แน่ใจว่าคุณได้ปฏิบัติตามขั้นตอนเหล่านี้:

- [แก้ไขปัญหาเครือข่ายที่แมปไดรฟ์ที่เชื่อมต่อกับ SharePoint Online](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [ข้อผิดพลาดการรับรองความถูกต้องจะเกิดขึ้นเมื่อไคลเอ็นต์ไม่มีการสนับสนุน TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**หมายเหตุ:** ถ้าคุณใช้ Internet Explorer 10กับ Windows 8 หรือ Windows 7 และได้รับ **การเข้าถึง** ถูกปฏิเสธหรือเส้นทางไม่สามารถเข้าถึงได้เมื่อแมปไดรฟ์ ให้แก้ไขปัญหานี้โดยการติดตั้งการแก้ไข [ด่วนนี้](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)