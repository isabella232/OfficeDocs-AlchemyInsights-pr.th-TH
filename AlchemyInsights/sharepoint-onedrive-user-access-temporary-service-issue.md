---
title: ปัญหาเกี่ยวกับประสิทธิภาพการSharePointหรือOneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093861"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePointหรือOneDriveช้า ไม่สามารถเข้าถึง หรือไม่พร้อมใช้งานได้โดยผู้ใช้หลายราย

If a OneDrive or SharePoint site is not available to multiple users who previously had access, may be a temporary service issue. [ตรวจสอบแดชบอร์ดสถานภาพ](https://portal.office.com/adminportal/home#/servicehealth)บริการ

**เพิ่มและสิทธิ์การใช้งานผู้ใช้**

ตรวจสอบให้แน่ใจว่าคุณ[กําหนดสิทธิ์การใช้งานให้กับผู้ใช้ใน Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**กําหนดสิทธิ์**

ถ้าผู้ใช้ได้รับการมอบหมายสิทธิ์การใช้งาน SharePoint และยังคงได้รับข้อความปฏิเสธการเข้าถึง โปรดตรวจสอบว่าพวกเขาได้รับมอบหมาย [ระดับ](https://docs.microsoft.com/sharepoint/understanding-permission-levels) สิทธิ์ที่เหมาะสม

**พิจารณาใช้ฟีเจอร์การร้องขอการเข้าถึง**

ฟีเจอร์ [การร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ช่วยให้บุคคลสามารถร้องขอการเข้าถึงเนื้อหาที่พวกเขาไม่มีสิทธิ์ในการดูได้ในขณะนี้

**อนุญาตสคริปต์แบบปรับแต่งเองอาจทําให้ปัญหาการเข้าถึงถูกปฏิเสธ**

มีบางสถานการณ์ที่ฟีเจอร์ *อนุญาตสคริปต์แบบ* ปรับแต่งเองอาจแสดงการเข้าถึงถูกปฏิเสธ For a list of features affected, security considerations and theability to disable the feature. โปรดไปที่ [อนุญาต หรือป้องกันสคริปต์แบบปรับแต่ง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)เอง

