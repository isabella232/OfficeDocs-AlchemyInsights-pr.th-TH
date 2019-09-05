---
title: ไม่มีการส่งการแจ้งเตือนการแจ้งเตือนของ SharePoint
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: d01d985f34d782fe14b3e2e6e6696c0101002db1
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36744660"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>ไม่มีการส่งการแจ้งเตือนการแจ้งเตือนของ SharePoint

กรุณาตรวจสอบโฟลเดอร์ขยะใน e-mail ของคุณเป็นบางครั้งการแจ้งเตือนอาจจะไปที่นั่น

ตรวจสอบว่าไม่มีการจัดส่งการ**แจ้งเตือนทั้งหมด**หรือถ้าไม่มี**การส่งการแจ้งเตือนแต่ละรายการ**จากแฟ้มหรือไลบรารีเฉพาะ

- การ**แจ้งเตือนแต่ละครั้งจะไม่มีการจัดส่ง**: ถ้าไม่มีการส่งการแจ้งเตือนแต่ละรายการจากแฟ้มหรือไลบรารีที่ระบุคุณสามารถพยายามลบและสร้างขึ้นใหม่ได้ ดู[จัดการดูหรือลบการแจ้งเตือนของ SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online)เพื่อสร้างการแจ้งเตือนใหม่
- การ**แจ้งเตือนทั้งหมดจะไม่ถูกส่ง**: ถ้าการแจ้งเตือนทั้งหมดจากหลายไฟล์หรือไลบรารีจะไม่ถูกส่งไปที่[แดชบอร์ดความสมบูรณ์ของบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อตรวจสอบคำแนะนำ/เหตุการณ์ที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange ปัญหานี้อาจจะมีความสามารถในการแจ้งเตือนของ SharePoint หรือล่าช้าในการส่งผ่านการแลกเปลี่ยน นอกจากนี้ยังจะเป็นสิ่งสำคัญที่จะทราบว่ามีการจัดส่งทาง e-mail อื่นๆและถ้าไม่ปัญหาที่มีแนวโน้มที่จะเกิดความล่าช้าของอัตราแลกเปลี่ยน

คำถามที่พบบ่อยเกี่ยวกับการแจ้งเตือน:

- ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้สนับสนุนเฉพาะกลุ่มการรักษาความปลอดภัยและ O365 เท่านั้น
- คุณไม่สามารถกำหนดเทมเพลตอีเมลแจ้งเตือนได้ คุณจำเป็นต้องใช้ Microsoft FLOW หรือ SharePoint Designer เวิร์กโฟลว์เพื่อให้บรรลุเป้าหมายเหล่านั้น

ข้อมูลเพิ่มเติม:

- **การตั้งค่าการแจ้งเตือน**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าการแจ้งเตือนโปรดดูที่การสร้างการแจ้ง[เตือนเพื่อรับการแจ้งให้ทราบเมื่อมีการเปลี่ยนแปลงแฟ้มหรือโฟลเดอร์ใน SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)
- **แก้ไขปัญหาการแจ้งเตือน**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการแก้ไขปัญหาการแจ้งเตือนให้ดูที่[ผู้ใช้ไม่ได้รับการแจ้งเตือนของ SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)
- **นโยบายการแจ้งเตือนการปฏิบัติตามกฎระเบียบของ O365 ขั้นสูง**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าการแจ้งเตือนเหล่านี้โปรดดูที่[นโยบายการแจ้งเตือนการปฏิบัติตามนโยบาย](https://docs.microsoft.com/office365/securitycompliance/alert-policies)
- **บันทึกการตรวจสอบ SharePoint และ OneDrive**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการกู้คืนเหตุการณ์เหล่านี้โปรดดู[ที่การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)
- ข้อความ**แจ้งเตือนที่ส่งโดยการป้องกันภัยคุกคามขั้นสูง**: ดู[ATP สำหรับ SharePoint และ OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)
- ข้อความ**แจ้งเตือนที่ส่งโดยตำรวจป้องกันข้อมูลสูญหาย**: ดู[การแจ้งเตือนทาง EMAIL สำหรับนโยบาย DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง

ต้องการลองการไหลของ Microsoft ใน SharePoint แบบออนไลน์หรือไม่

- [สร้างโฟลว์](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint และการไหล](https://flow.microsoft.com//blog/sharepoint-and-flow/)
