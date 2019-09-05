---
title: สร้างไซต์ใน SharePoint แบบออนไลน์
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755327"
---
# <a name="create-sharepoint-sites-using-templates"></a>สร้างไซต์ SharePoint โดยใช้แม่แบบ

แม่แบบไซต์ SharePoint เป็นคำนิยามที่สร้างไว้ล่วงหน้าซึ่งออกแบบมาโดยรอบความต้องการทางธุรกิจที่เฉพาะเจาะจง สำหรับข้อมูลเพิ่มเติมให้ดู[การใช้แม่แบบเพื่อสร้างไซต์ SharePoint ชนิดต่างๆ](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

ต่อไปนี้เป็นปัญหา/วิธีแก้ไขทั่วไปบางอย่างเกี่ยวกับการบันทึกไซต์หรือรายการเป็นแม่แบบใน Sharepoint แบบออนไลน์ 

**บันทึกปุ่มแม่แบบไซต์/รายการไม่พร้อมใช้งานหรือหายไป**

ผู้ดูแลระบบจะต้องอนุญาตสคริปต์ที่กำหนดเองเพื่อเปิดใช้งานคุณลักษณะแม่แบบ สำหรับขั้นตอนโดยละเอียดตัวอย่างและข้อควรพิจารณาที่เห็น 

- [อนุญาตหรือป้องกันสคริปต์ที่กำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- คำสั่งบันทึกไซต์เป็นแม่แบบไม่ได้รับการสนับสนุนและอาจทำให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐานการประกาศของเซิร์ฟเวอร์ SharePoint

**ไม่สามารถสร้างแม่แบบไซต์หรือทำงานไม่ถูกต้อง**

แม่แบบอาจจะหายไป[คุณลักษณะ](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)และจะไม่เปิดใช้งาน ถ้าคุณลักษณะนี้ไม่พร้อมใช้งานสำหรับการเปิดใช้งานในไซต์คอลเลกชันปัจจุบันคุณจะไม่สามารถใช้แม่แบบไซต์เพื่อสร้างไซต์ได้

- ตรวจสอบเพื่อดูว่ารายการหรือไลบรารีใดๆเกิน[ขีดจำกัดมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)จำกัดของรายการ๕๐๐๐เช่นนี้สามารถบล็อกการสร้างแม่แบบไซต์

- ไซต์นี้อาจใช้ทรัพยากรมากเกินไปและแม่แบบไซต์เกินขีดจำกัด๕๐ MB


- มีปัญหาในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์การค้นหา สำหรับข้อมูลเพิ่มเติมให้ดู[รายการที่สร้างขึ้นโดยแม่แบบไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและวิธีแก้ไขทั่วไปโปรดตรวจสอบ[สร้างและใช้แม่แบบไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



