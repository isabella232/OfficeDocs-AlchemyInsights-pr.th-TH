---
title: ผู้ใช้คนเดียวไม่เห็น Add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198222"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>ผู้ใช้คนเดียวไม่เห็น Add-in ใน Outlook

ผู้ใช้อาจเป็นส่วนหนึ่งของบทบาทที่ไม่มีพารามิเตอร์ AppsForOfficeEnabled ที่ถูกต้อง เรียกใช้ cmdlet นี้เพื่อดูว่าบทบาทที่ถูกต้องเกี่ยวข้องกับผู้ใช้:

รับ-การจัดการการจัดระเบียบ -บทบาทอัสสิกนีuser@domain.com -delegating $false | รูปแบบตาราง - บทบาทอัตโนมัติ,บทบาทสมการชื่อ,สมอสมจณีพิมพ์

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ Add-in สําหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)
