---
title: ปัญหาประสิทธิภาพการทํางาน-SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511167"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint หรือ OneDrive ช้า ไม่สามารถเข้าถึง หรือไม่พร้อมใช้งานสําหรับผู้ใช้หลายคน

ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสําหรับผู้ใช้หลายคนที่เคยมีการเข้าถึง อาจมีปัญหาการบริการชั่วคราว [ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)

**เพิ่มและอนุญาตให้ใช้สิทธิของผู้ใช้**

ให้แน่ใจว่าคุณ[กําหนดสิทธิ์การใช้งานให้กับผู้ใช้ใน Microsoft 365 สําหรับธุรกิจ](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**กําหนดสิทธิ์**

ถ้าผู้ใช้ได้รับมอบหมายสิทธิ์การใช้งาน Sharepoint และยังคงได้รับข้อความปฏิเสธการเข้าถึง โปรดตรวจสอบให้แน่ใจว่าผู้ใช้ได้รับ[มอบหมายระดับสิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**พิจารณาใช้คุณลักษณะคําขอการเข้าถึง**

[คุณลักษณะคําขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)อนุญาตให้ผู้ใช้ร้องขอการเข้าถึงเนื้อหาที่พวกเขาไม่มีสิทธิ์เห็นในขณะนี้

**อนุญาตสคริปต์แบบกําหนดเองอาจทําให้เกิดปัญหาการเข้าถึงถูกปฏิเสธ**

มีบางสถานการณ์ที่คุณลักษณะ*อนุญาตสคริปต์แบบกําหนดเอง*อาจนําเสนอการเข้าถึงถูกปฏิเสธ สําหรับรายการของคุณลักษณะที่ได้รับผลกระทบ กรุณาเยี่ยมชม[อนุญาตหรือป้องกันสคริปต์ที่กําหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

