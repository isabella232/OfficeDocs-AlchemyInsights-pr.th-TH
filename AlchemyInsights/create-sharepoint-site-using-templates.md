---
title: การสร้างไซต์ใน SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732262"
---
# <a name="create-sharepoint-sites-using-templates"></a>การสร้างไซต์ SharePoint โดยใช้เทมเพลต

ความสามารถในการบันทึกไซต์เป็นเทมเพลตจะไม่ได้รับการสนับสนุนด้วยการติดต่อสื่อสารหรือไซต์ทีมที่ทันสมัย สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการใช้เทมเพลตให้ดูที่[บันทึกดาวน์โหลดและอัปโหลดไซต์ SharePoint เป็นเทมเพลต](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)

ต่อไปนี้เป็นปัญหาทั่วไป/วิธีแก้ไขปัญหาทั่วไปเกี่ยวกับการบันทึกไซต์หรือรายการเป็นเทมเพลตใน Sharepoint Online 

**ปุ่มบันทึกเทมเพลตไซต์/รายการไม่พร้อมใช้งานหรือหายไป**

ผู้ดูแลระบบจะต้องเปิดใช้งานสคริปต์แบบกำหนดเองเพื่อเปิดใช้งานฟีเจอร์เทมเพลต สำหรับขั้นตอนโดยละเอียดตัวอย่างและข้อควรพิจารณา 

- [อนุญาตหรือป้องกันสคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- คำสั่งบันทึกไซต์เป็นเทมเพลตจะไม่ได้รับการสนับสนุนและอาจทำให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐานของการประกาศของ SharePoint Server

**ไม่สามารถสร้างเทมเพลตของไซต์หรือทำงานได้อย่างถูกต้อง**

เทมเพลตนี้อาจไม่มี [ฟีเจอร์](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) และไม่สามารถเปิดใช้งานได้ ถ้าฟีเจอร์ไม่พร้อมใช้งานเมื่อต้องการเปิดใช้งานในไซต์คอลเลกชันปัจจุบันคุณจะไม่สามารถใช้เทมเพลตของไซต์เพื่อสร้างไซต์ได้

- ตรวจสอบดูว่ารายการหรือไลบรารีใดที่เกินขีด [จำกัดของมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ของรายการ๕๐๐๐เนื่องจากการทำเช่นนี้สามารถบล็อกการสร้างเทมเพลตของไซต์ได้

- ไซต์อาจใช้แหล่งข้อมูลมากเกินไปและดังนั้นแม่แบบไซต์เกินขีดจำกัด๕๐ MB


- มีปัญหาเกิดขึ้นในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์การค้นหา สำหรับข้อมูลเพิ่มเติมให้ดูที่[รายการที่สร้างขึ้นโดยใช้เทมเพลตไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับปัญหาทั่วไปและการแก้ไขปัญหาโปรดตรวจสอบการ[สร้างและใช้เทมเพลตของไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



