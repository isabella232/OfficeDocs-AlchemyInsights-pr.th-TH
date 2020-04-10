---
title: ตั้งค่าใบรับรอง APNS ของ iOS Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 027e1e0fa3b625fa0f619bc6d74844f6ec5be769
ms.sourcegitcommit: 75346a972c2174248de3bb55a19d714cee43c1cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/09/2020
ms.locfileid: "43211433"
---
# <a name="intune-ios-set-up-apns-certificate"></a>ตั้งค่าใบรับรอง APNS ของ iOS Intune

ใบรับรอง Apple MDM Push (หรือที่เรียกว่าใบรับรองบริการแจ้งเตือนแบบพุช (APNS) ของ Apple) ยังไม่ได้รับการกําหนดค่าในการสมัครใช้งานของคุณ

หากไม่มีการกําหนดค่าใบรับรอง Apple MDM Push คุณจะไม่สามารถลงทะเบียนและจัดการอุปกรณ์ iOS และ MacOS ได้ หลังจากที่คุณเพิ่มใบรับรองไปยัง Intune ผู้ใช้ของคุณสามารถติดตั้งแอปพอร์ทัลของบริษัทเพื่อลงทะเบียนอุปกรณ์ iOS ของตนได้

สําหรับคําแนะนําทีละขั้นตอนในการเพิ่มใบรับรอง APNS กับผู้เช่า Intune ของคุณ โปรดตรวจทานเนื้อหาในการเชื่อมโยงต่อไปนี้:

- [รับใบรับรองการผลักดัน MDM ของ Apple](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

หากคุณมีปัญหากับใบรับรองการแจ้งเตือนแบบพุชของ Apple (APNs) โปรดดูโพสต์บล็อกนี้: [Intune และใบรับรอง APNs: คําถามที่ถามบ่อยและปัญหาทั่วไป](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)
