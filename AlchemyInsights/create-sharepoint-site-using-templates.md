---
title: สร้างไซต์ใน SharePoint แบบออนไลน์
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770442"
---
# <a name="create-sharepoint-sites-using-templates"></a>การสร้างไซต์ SharePoint โดยใช้แม่แบบ

ความสามารถในการบันทึกไซต์เป็นแม่แบบไม่ได้รับการสนับสนุนด้วยการสื่อสารที่ทันสมัยหรือเว็บไซต์ทีม สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการใช้แม่แบบดู[บันทึกดาวน์โหลดและอัปโหลดไซต์ SharePoint เป็นแม่แบบ](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)

ต่อไปนี้เป็นปัญหาทั่วไปบางส่วน/การแก้ไขปัญหาเกี่ยวกับการบันทึกไซต์หรือรายการเป็นแม่แบบใน Sharepoint แบบออนไลน์ 

**บันทึกปุ่มแม่แบบของไซต์/รายการไม่พร้อมใช้งานหรือหายไป**

ผู้ดูแลระบบจะต้องอนุญาตให้สคริปต์ที่กำหนดเองเพื่อเปิดใช้งานคุณลักษณะแม่แบบ สำหรับขั้นตอนโดยละเอียดตัวอย่างและข้อควรพิจารณา 

- [อนุญาตหรือป้องกันสคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- คำสั่งบันทึกไซต์เป็นแม่แบบไม่ได้รับการสนับสนุนและอาจทำให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐานการเผยแพร่เซิร์ฟเวอร์ SharePoint

**ไม่สามารถสร้างแม่แบบไซต์หรือทำงานไม่ถูกต้อง**

แม่แบบอาจขาด[คุณลักษณะ](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)และจะไม่เปิดใช้งาน ถ้าคุณลักษณะไม่พร้อมใช้งานเมื่อต้องการเปิดใช้งานในไซต์คอลเลกชันปัจจุบันคุณจะไม่สามารถใช้แม่แบบไซต์เพื่อสร้างไซต์ได้

- ตรวจสอบดูว่ามีรายการหรือไลบรารีเกินขีด[จำกัดของมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)ของ๕๐๐๐รายการในขณะนี้สามารถบล็อกการสร้างแม่แบบไซต์

- ไซต์อาจใช้ทรัพยากรมากเกินไปและดังนั้นแม่แบบไซต์เกินขีดจำกัด๕๐ MB


- มีปัญหาในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์การค้นหา สำหรับข้อมูลเพิ่มเติมให้ดูที่[รายการสร้างแม่แบบไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

สำหรับข้อมูลรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและวิธีการแก้ไขทั่วไปโปรดตรวจสอบการ[สร้างและใช้แม่แบบไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



