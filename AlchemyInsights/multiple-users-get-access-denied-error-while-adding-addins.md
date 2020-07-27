---
title: ผู้ใช้หลายคนได้รับข้อผิดพลาดการเข้าถึงถูกปฏิเสธในขณะที่เพิ่ม Add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424177"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>ผู้ใช้หลายคนได้รับข้อผิดพลาดการเข้าถึงถูกปฏิเสธในขณะที่เพิ่ม Add-in ใน Outlook

คุณสามารถระบุผู้ดูแลระบบในองค์กรของคุณมีสิทธิ์ในการติดตั้งและจัดการ Add-in สําหรับ Outlook คุณยังสามารถระบุผู้ใช้ในองค์กรของคุณที่มีสิทธิ์ในการติดตั้งและจัดการ Add-in สําหรับการใช้ของตนเอง

สําหรับรายละเอียด ให้ดูที่[ระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ Add-in สําหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)

เมื่อต้องการตรวจสอบว่า คุณได้กําหนดสิทธิ์สําหรับผู้ใช้เสร็จเรียบร้อยแล้ว ให้แทนที่ <Role Name> ด้วยชื่อของบทบาทเพื่อตรวจสอบ และเรียกใช้คําสั่งต่อไปนี้ใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน:

รับการจัดการการจัดระเบียบ -บทบาท <Role Name> "" -GetประสิทธิภาพUsers

ตัวอย่างนี้แสดงวิธีการตรวจสอบว่าคุณได้กําหนดสิทธิ์ให้ใครติดตั้ง Add-in จาก Office Store สําหรับองค์กร

Powershell

บทบาท "Org Marketplace Apps" - Getประสิทธิภาพการใช้งาน

ในผลลัพธ์ที่ได้รับการจัดการรายงานการตรวจสอบรายการในคอลัมน์ผู้ใช้ที่มีประสิทธิภาพ

สําหรับข้อมูลไวยากรณ์และพารามิเตอร์โดยละเอียด ให้ดูที่[รับการจัดการการมอบหมาย](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)
 