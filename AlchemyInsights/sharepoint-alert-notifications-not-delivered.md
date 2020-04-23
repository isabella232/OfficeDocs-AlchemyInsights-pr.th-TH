---
title: การแจ้งเตือนของ SharePoint ไม่ถูกจัดส่ง
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742066"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>การแจ้งเตือนของ SharePoint ไม่ถูกจัดส่ง

โปรดตรวจสอบโฟลเดอร์อีเมลขยะในอีเมลของคุณเนื่องจากบางครั้งการแจ้งเตือนอาจไปที่นั่น

กําหนดว่าการแจ้งเตือน**ทั้งหมดจะไม่ส่ง**หรือถ้า**การแจ้งเตือนแต่ละรายการ**จากแฟ้มหรือไลบรารีที่ระบุไม่ได้ถูกส่ง

- **การแจ้งเตือนแต่ละข้อความจะไม่ถูกส่ง**: หากการแจ้งเตือนแต่ละตัวจากแฟ้มหรือไลบรารีที่ระบุไม่ได้ถูกส่ง ดู[จัดการ ดู หรือลบการแจ้งเตือนของ SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)เพื่อสร้างการแจ้งเตือนใหม่
- **การแจ้งเตือนทั้งหมดจะไม่ส่ง**: ถ้าการแจ้งเตือนทั้งหมดจากหลายแฟ้มหรือไลบรารีไม่ได้ส่ง ไปที่[แดชบอร์ดของสถานบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อตรวจสอบคําแนะนํา/เหตุการณ์ใด ๆ ที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange ปัญหาอาจอยู่กับความสามารถของการแจ้งเตือน SharePoint หรือความล่าช้าในอีเมลผ่านอัตราแลกเปลี่ยน นอกจากนี้ยังจะเป็นสิ่งสําคัญที่จะทราบว่าอีเมลอื่น ๆ จะถูกจัดส่งและถ้าไม่ปัญหามีแนวโน้มความล่าช้าของอัตราแลกเปลี่ยน

คําถามที่พบบ่อยเกี่ยวกับการแจ้งเตือน:

- ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้ เฉพาะกลุ่ม Security และ O365 เท่านั้น
- คุณไม่สามารถกําหนดแม่แบบอีเมลการแจ้งเตือนเองได้ คุณต้องใช้กระแสของ Microsoft หรือเวิร์กโฟลว์ SharePoint Designer เพื่อให้บรรลุผลเหล่านั้น

ข้อมูลเพิ่มเติม:

- **การตั้งค่าการแจ้งเตือน**: สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าการแจ้งเตือน ให้ดูที่[การสร้างการแจ้งเตือนเพื่อรับการแจ้งเตือนเมื่อมีการเปลี่ยนแปลงแฟ้มหรือโฟลเดอร์ใน SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)
- **การแก้ไขปัญหาการแจ้งเตือน**: สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการแก้ไขปัญหาการแจ้งเตือน ให้ดูที่[ผู้ใช้ไม่ได้รับการแจ้งเตือนการแจ้งเตือนของ SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)
- **นโยบายการแจ้งเตือนการปฏิบัติตามกฎระเบียบ O365 ขั้นสูง**: สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าการแจ้งเตือนเหล่านี้ โปรดดู[นโยบายการแจ้งเตือนการปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/office365/securitycompliance/alert-policies)
- **SharePoint และ OneDrive ตรวจสอบแฟ้มบันทึก**: สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการเรียกเหตุการณ์เหล่านี้ ให้ดูที่[ค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)
- **การแจ้งเตือนที่ส่งโดยการป้องกันภัยคุกคามขั้นสูง**: ดู[ATP สําหรับ SharePoint และ OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)
- **การแจ้งเตือนที่ส่งโดยตํารวจป้องกันการสูญหายของข้อมูล**: ดู[การแจ้งเตือนทางอีเมลสําหรับนโยบาย DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง

ต้องการลอง Microsoft ไหลใน SharePoint แบบออนไลน์หรือไม่

- [สร้างโฟลว์](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint และโฟลว์](https://flow.microsoft.com//blog/sharepoint-and-flow/)
