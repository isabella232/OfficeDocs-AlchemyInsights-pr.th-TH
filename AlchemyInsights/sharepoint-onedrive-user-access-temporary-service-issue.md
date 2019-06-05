---
title: ปัญหาเกี่ยวกับประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719535"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint หรือ OneDrive ช้า ไม่สามารถเข้าถึง หรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน

ถ้าไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้ มีการเข้าถึงไซต์ SharePoint หรือการ OneDrive อาจมีปัญหากับบริการชั่วคราว [ตรวจสอบแดชบอร์ความสมบูรณ์ของการบริการ](https://portal.office.com/adminportal/home#/servicehealth)

## <a name="add-and-license-the-user"></a>เพิ่ม และสิทธิ์การใช้งานของผู้ใช้

ให้แน่ใจว่าคุณ[กำหนดสิทธิ์การใช้งานสำหรับผู้ใช้ใน Office 365 สำหรับธุรกิจ](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)


## <a name="assign-permissions"></a>กำหนดการอนุญาต

ถ้าผู้ใช้มีการกำหนดสิทธิ์การใช้งาน Sharepoint และยังคงได้รับการเข้าถึงถูกปฏิเสธข้อความ โปรดให้แน่ใจว่า พวกเขาได้[ระดับของสิทธิ์ที่](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)กำหนดให้

## <a name="consider-using-the-access-request-feature"></a>พิจารณาการใช้คุณลักษณะการร้องขอการเข้าถึง

การ[เข้าถึงลักษณะการทำงานขอ](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)อนุญาตให้บุคคลที่จะร้องขอการเข้าถึงเนื้อหาที่พวกเขายังไม่ได้รับอนุญาตให้ดู

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>อนุญาตให้ใช้สคริปต์แบบกำหนดเองอาจทำให้เกิดปัญหาปฏิเสธการเข้าถึง

มีบางสถานการณ์ที่คุณลักษณะที่*อนุญาตให้สคริปต์ที่กำหนดเอง*อาจจะนำเสนอการเข้าถึงถูกปฏิเสธ สำหรับรายการของลักษณะการทำงานที่ได้รับผลกระทบ ข้อควรพิจารณาด้านความปลอดภัย และความสามารถในการปิดใช้งานลักษณะการทำงาน โปรดเยี่ยมชม[อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)

