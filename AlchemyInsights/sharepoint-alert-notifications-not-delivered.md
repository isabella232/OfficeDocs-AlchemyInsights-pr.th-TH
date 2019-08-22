---
title: แจ้งเตือน SharePoint ไม่ได้จัดส่ง
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
ms.openlocfilehash: f389785fcd1029ae5a47e07c723874f9f214109d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504482"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>แจ้งเตือน SharePoint ไม่ได้จัดส่ง

โปรดตรวจสอบโฟลเดอร์อีเมลขยะในอีเมลของคุณ ในขณะที่บางครั้งข้อความแจ้งเตือนอาจไปมี

กำหนดว่าถ้า**ไม่ได้จัดส่งข้อความแจ้งเตือนทั้งหมด**หรือถ้าไม่ได้ส่ง**ข้อความแจ้งเตือนแต่ละรายการ**จากแฟ้มใดแฟ้มหนึ่งหรือไลบรารี

- **ไม่ได้จัดส่งข้อความแจ้งเตือนแต่ละ**: ถ้าไม่มีส่งข้อความแจ้งเตือนจากแฟ้มใดแฟ้มหนึ่งหรือไลบรารีแต่ละ คุณสามารถพยายามที่จะลบ และสร้างใหม่ดังกล่าวได้ ดูการ[จัดการ ดู หรือลบการแจ้งเตือนของ SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online)เมื่อต้องการสร้างการแจ้งเตือน
- **ไม่ได้จัดส่งข้อความแจ้งเตือนทั้งหมด**: ถ้าไม่ส่งข้อความแจ้งเตือนทั้งหมดจากแฟ้มหรือไลบรารีหลาย เยี่ยมชม[แดชบอร์ดบริการสุขภาพ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อตรวจหาใด ๆ คำแนะนำสำหรับ/ปัญหาที่อาจเกิดขึ้นกับ SharePoint หรือแลกเปลี่ยน ปัญหานี้อาจจะ มีความสามารถแจ้งเตือนของ SharePoint หรือความล่าช้าในอีเมล์โดยใช้อัตราแลกเปลี่ยน ก็จะเป็นสิ่งสำคัญที่ต้องหมายเหตุ ว่า กำลังถูกส่งทางอีเมลอื่น ๆ และถ้าไม่ ปัญหาอาจ มีความล่าช้าในการแลกเปลี่ยน

FAQ เกี่ยวกับการแจ้งเตือน:

- ไม่สามารถส่งข้อความแจ้งเตือนไปยัง กลุ่มการแจกจ่าย การรักษาความปลอดภัยเท่านั้น และกลุ่ม O365 ได้รับการสนับสนุน
- คุณไม่สามารถกำหนดแม่แบบอีเมลที่แจ้งเตือน คุณจำเป็นต้องใช้ขั้นตอน Microsoft หรือ SharePoint Designer ลำดับบรรลุถึง

หากต้องการข้อมูลเพิ่มเติม:

- **การตั้งค่าการแจ้งเตือน**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าการแจ้งเตือน ดูที่การ[สร้างข้อความแจ้งเตือนเพื่อรับการแจ้งเตือนเมื่อมีการเปลี่ยนแปลงแฟ้มหรือโฟลเดอร์ใน SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)
- **แก้ไขการแจ้งเตือน**: ดูข้อมูลเพิ่มเติมเกี่ยวกับการแก้ปัญหาการแจ้งเตือน[ผู้ใช้ที่ไม่ได้รับการแจ้งเตือนของ SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)
- **ขั้นสูงแจ้งเตือนนโยบายปฏิบัติตามกฎระเบียบ O365**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าการแจ้งเตือนเหล่านี้ ดู[นโยบายแจ้งเตือนการปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/office365/securitycompliance/alert-policies)
- **SharePoint และแฟ้มบันทึกการตรวจสอบ OneDrive**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการรับเหตุการณ์เหล่านี้ ให้ดู[บันทึกการตรวจสอบการค้นหา](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)
- **ส่งข้อความแจ้งเตือนโดยการป้องกันการคุกคามขั้นสูง**: ดู[ATP สำหรับ SharePoint และ OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)
- **ข้อความแจ้งเตือนที่ถูกส่งโดยป้องกันการสูญหายของข้อมูลด้านนโยบาย**: ดูการ[แจ้งเตือนทางอีเมลสำหรับนโยบาย DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)

## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง

ต้องการลองกระแส Microsoft ใน SharePoint แบบออนไลน์หรือไม่

- [สร้างขั้นตอน](https://support.office.com/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint และขั้นตอน](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)
