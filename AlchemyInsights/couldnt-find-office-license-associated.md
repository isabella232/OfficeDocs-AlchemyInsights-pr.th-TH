---
title: การแก้ไขMicrosoft 365ไม่พบข้อความที่เกี่ยวข้องของสิทธิ์การใช้งาน Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069623"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>การแก้ไขMicrosoft 365 "ไม่พบสิทธิ์การใช้งาน Office ที่เชื่อมโยงกัน"

ถ้าคุณได้รับข้อความนี้ ให้ลองวิธีต่อไปนี้:

1. ตรวจสอบการตั้งค่าไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตMicrosoft 365แอปของคุณ ให้ดูที่[Microsoft 365 URL และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user. 
3. เปิดแอป Office[และ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)ลงชื่อออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่
4. ไปที่ Windows การตั้งค่า >**บัญชี**  >  **อีเมล& บัญชี** และเอาบัญชีที่งานทั้งหมดออก ยกเว้นบัญชีที่ได้รับผลกระทบ
5. ไปที่ Windows การตั้งค่า >**การเข้าถึง**  >  **บัญชีที่ที่โรงเรียน** หรือที่โรงเรียน แล้วยกเลิกการเชื่อมต่อบัญชีที่งานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ
6. ตั้งค่าสถานะOfficeเปิดใช้งานใหม่ [เรียนรู้วิธีการ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [ลงชื่อเข้าใช้](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ

For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).