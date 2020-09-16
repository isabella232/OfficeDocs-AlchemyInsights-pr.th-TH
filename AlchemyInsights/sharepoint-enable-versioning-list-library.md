---
title: การกำหนดเวอร์ชันใน SharePoint และ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.custom:
- "5300025"
- "1702"
ms.openlocfilehash: 12207efc9822be6cf096fa4884a3cd244a286cbe
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800843"
---
# <a name="versioning-in-sharepoint-and-onedrive"></a>การกำหนดเวอร์ชันใน SharePoint และ OneDrive 


เมื่อเปิดใช้งานการกำหนดเวอร์ชันในรายการหรือไลบรารี SharePoint ของคุณคุณสามารถจัดเก็บติดตามและคืนค่ารายการในรายการและไฟล์ในไลบรารีได้เมื่อใดก็ตามที่มีการเปลี่ยนแปลง การกำหนดเวอร์ชันที่รวมเข้ากับการตั้งค่าอื่นๆเช่นเช็คเอาท์จะทำให้คุณสามารถควบคุมเนื้อหาที่โพสต์บนไซต์ของคุณได้มากและสามารถระบุค่าจริงได้ถ้าคุณต้องการดูหรือคืนค่าเวอร์ชันเก่าของรายการหรือไฟล์

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการกำหนดเวอร์ชันโปรดเยี่ยมชมบทความด้านล่าง

- [การกำหนดเวอร์ชันทำงานอย่างไรในรายการหรือไลบรารี SharePoint](https://support.office.com/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247)

- [การเปิดใช้งานและกำหนดค่าการกำหนดเวอร์ชันสำหรับรายการหรือไลบรารี](https://support.office.com/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f)

- [วิธีการดูประวัติเวอร์ชัน](https://support.office.com/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1)

- [คืนค่าไฟล์เวอร์ชันก่อนหน้าใน OneDrive](https://support.office.com/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893)

- [ดูไฟล์ Office เวอร์ชันก่อนหน้า](https://support.office.com/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2)

- [ขีดจำกัดการกำหนดเวอร์ชัน](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)

>[!Note] 
>ถ้าคุณเป็นลูกค้า Microsoft ๓๖๕การกำหนดเวอร์ชันจะเปิดใช้งานตามค่าเริ่มต้นเมื่อคุณสร้างไลบรารี OneDrive for Business ใหม่และจะบันทึกเวอร์ชัน๕๐๐ของเอกสารล่าสุดโดยอัตโนมัติ การทำเช่นนี้จะช่วยให้คุณป้องกันไม่ให้เอกสารหรือข้อมูลที่สำคัญสูญหาย ถ้าคุณมีไลบรารีที่มีอยู่บนไซต์ OneDrive for Business ของคุณหรือบนไซต์ทีมของคุณที่ไม่ได้เปิดใช้งานการกำหนดเวอร์ชันคุณสามารถเปิดใช้งานการกำหนดเวอร์ชันสำหรับพวกเขาได้ตลอดเวลา


