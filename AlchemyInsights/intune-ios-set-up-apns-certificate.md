---
title: การตั้งค่าใบรับรอง APN iOS ของ Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: f58405de018c916e08672022bb4f66292524b736
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667465"
---
# <a name="intune-ios-set-up-apns-certificate"></a>การตั้งค่าใบรับรอง APN iOS ของ Intune

ใบรับรองแบบพุชของ Apple MDM (หรือที่เรียกว่าใบรับรองบริการการแจ้งเตือนแบบพุชของ Apple (APN)) ไม่ได้ถูกกำหนดค่าในการสมัครใช้งานของคุณ

ถ้าไม่มีการกำหนดค่าใบรับรองแบบผลักข้อมูลของ Apple MDM คุณจะไม่สามารถลงทะเบียนและจัดการอุปกรณ์ iOS และ MacOS ได้ หลังจากที่คุณเพิ่มใบรับรองไปยัง Intune แล้วผู้ใช้ของคุณสามารถติดตั้งแอป Portal ของบริษัทเพื่อลงทะเบียนอุปกรณ์ iOS ของพวกเขาได้

สำหรับคำแนะนำทีละขั้นตอนในการเพิ่มใบรับรอง APN ให้กับผู้เช่า Intune ของคุณโปรดตรวจทานเนื้อหาบนลิงก์ต่อไปนี้:

- [รับใบรับรองแบบพุชของ Apple MDM](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

ถ้าคุณกำลังมีปัญหาเกี่ยวกับใบรับรองการแจ้งเตือนแบบพุชของ Apple (Apn) อ้างอิงไปยังโพสต์ในบล็อกนี้: [Intune และใบรับรอง apn: คำถามที่ถามบ่อยและปัญหาทั่วไป](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)
