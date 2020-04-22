---
title: ปัญหาประสิทธิภาพการทํางาน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: ec378981d4f24837b037e18214cbeba2f2b657c5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692712"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint หรือ OneDrive ช้า ไม่สามารถเข้าถึง หรือไม่พร้อมใช้งานสําหรับผู้ใช้หลายคน

ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสําหรับผู้ใช้หลายคนที่ก่อนหน้านี้มีการเข้าถึง อาจมีปัญหาการบริการชั่วคราว [ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)

**เพิ่มและอนุญาตผู้ใช้**

ตรวจสอบให้แน่ใจว่าคุณ[กําหนดสิทธิ์การใช้งานให้กับผู้ใช้ใน Microsoft 365 สําหรับธุรกิจ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)


**กําหนดสิทธิ์**

ถ้าผู้ใช้ได้รับมอบหมายสิทธิ์การใช้งาน Sharepoint และยังคงได้รับข้อความปฏิเสธการเข้าถึง โปรดตรวจสอบให้แน่ใจว่าผู้ใช้ได้รับ[สิทธิ์ที่เหมาะสมที่กําหนด](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**พิจารณาการใช้คุณลักษณะการร้องขอการเข้าถึง**

[คุณลักษณะการร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)อนุญาตให้บุคคลอื่นร้องขอการเข้าถึงเนื้อหาที่ไม่ได้รับอนุญาติให้ดูในขณะนี้

**อนุญาตสคริปต์แบบกําหนดเองอาจทําให้เกิดปัญหาการเข้าถึงถูกปฏิเสธ**

มีบางสถานการณ์ที่คุณลักษณะ*การอนุญาตให้สคริปต์แบบกําหนดเอง*อาจนําเสนอการเข้าถึงถูกปฏิเสธ สําหรับรายการของคุณลักษณะที่ได้รับผลกระทบข้อควรพิจารณาด้านความปลอดภัยและความสามารถในการปิดใช้งานคุณลักษณะ กรุณาเยี่ยมชม[อนุญาตหรือป้องกันสคริปต์ที่กําหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

