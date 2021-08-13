---
title: การเกษียณบริการการเข้าถึง
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938714"
---
# <a name="access-services-retirement"></a>การเกษียณบริการการเข้าถึง

ดังที่เราประกาศครั้งแรกใน MC97576 ในเดือนมีนาคม 2017 และยังคงสื่อสารในช่วงปีที่ผ่านมาAccess Servicesเลิกใช้ ขั้นตอนถัดไปในกระบวนการนี้จะเป็นการลบฐานข้อมูลเว็บ Access ที่ใช้รายการฐานข้อมูลSharePointเป็นที่เก็บข้อมูลหลัก

**สิ่งนี้มีผลต่อฉันอย่างไร**

ตั้งแต่เดือนมิถุนายน 2019 เราจะหยุดการสร้างฐานข้อมูล Access ใหม่ใน SharePoint Online และปิดบริการและแอปที่เหลือภายในเดือนเมษายน 2020

**ฉันต้องเตรียมตัวอย่างไรกับการเปลี่ยนแปลงนี้**

เราขอสนับสนุนให้คุณสร้างแผนการเปลี่ยนภาพให้กับฐานข้อมูล Access บนเว็บขององค์กรของคุณ ผู้ดูแลระบบสามารถใช้สแกนเนอร์SharePoint [Access ของคุณ](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)เพื่อรับสินค้าคงคลังของแอป Access ที่ไซต์ใช้อยู่

มีหลายวิธีในการโยกย้ายข้อมูลฐานข้อมูลเว็บ Access:

- การนําเข้าไปยังฐานข้อมูล Access ภายในเครื่อง (. ACCDB) หรือExcelไฟล์
- นอกจากนี้ เราขอแนะMicrosoft PowerAppsวิธีแก้ไขปัญหาทางธุรกิจที่เป็นแพลตฟอร์มอื่นเพื่อสร้างโซลูชันทางธุรกิจแบบไม่มีรหัสให้กับเว็บและอุปกรณ์เคลื่อนที่