---
title: จัดการ Schema การค้นหาใน SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 8eb0e93ea5bbf2154213274041b28a3c908090dae724b8f8e55fa2fb05f16d86
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085103"
---
# <a name="manage-search-schema-in-sharepoint-online"></a>จัดการ Schema การค้นหาใน SharePoint Online

Schema การค้นหาจะควบคุมสิ่งที่ผู้ใช้สามารถค้นหา ได้ วิธีที่ผู้ใช้สามารถค้นหา และวิธีที่คุณสามารถแสดงผลลัพธ์บนเว็บไซต์การค้นหาของคุณ 

ให้ดูที่[จัดการ Schema การค้นหาใน SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema)เพื่อเรียนรู้วิธีการ: 
- เปลี่ยน Schema การค้นหา
- สร้างคุณสมบัติที่มีการจัดการ
- แมปคุณสมบัติที่ตระเวนของแผนที่ไปยังคุณสมบัติที่มีการจัดการ

โปรดสังเกตสิ่งต่อไปนี้เกี่ยวกับการจัดการ Schema การค้นหาของคุณ

- ถ้าคุณได้รับคําเตือนที่ระบุว่า **แอปพลิเคชันถูก** หยุดชั่วคราวเมื่อเปลี่ยน Schema นี่จะเกิดขึ้นชั่วคราวเท่านั้นเมื่อมีการบํารุงรักษาบริการเกิดขึ้น 

    ถ้าเวลาผ่านไปมากกว่า 24 ชั่วโมงแล้วคุณยังคงได้รับคําเตือน โปรดบันทึกกรณีสนับสนุน
- When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled. In SharePoint Online, crawling happens automatically based on the defined crawl schedule.
- To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) 

For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) 


