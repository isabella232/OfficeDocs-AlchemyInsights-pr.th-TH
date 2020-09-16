---
title: ส่งการแจ้งเตือนแบบกำหนดเองด้วย Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720665"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>วิธีการส่งการแจ้งเตือนแบบกำหนดเองไปยังผู้ใช้ของอุปกรณ์ iOS และ Android ที่มีการจัดการ

การแจ้งเตือนแบบกำหนดเองสำหรับ Intune จะถูกประมวลผลโดยแอปพอร์ทัลของบริษัทบนอุปกรณ์ของผู้ใช้ แอปจะสร้างการแจ้งเตือนแบบพุชบนอุปกรณ์นั้น

ต่อไปนี้คือข้อกำหนดเบื้องต้นของอุปกรณ์เพื่อสนับสนุนการรับการแจ้งเตือนแบบกำหนดเองและสำหรับแอปเพื่อสร้างการแจ้งเตือนแบบพุช:

- อุปกรณ์จำเป็นต้องติดตั้งแอปพอร์ทัลบริษัท  

- อุปกรณ์ต้องอนุญาตให้แอป Portal ของบริษัทส่งการแจ้งเตือนแบบพุช เมื่อแอปได้รับการติดตั้งหรืออัปเดตโปรแกรมจะพร้อมท์ให้ผู้ใช้อนุญาตการแจ้งให้ทราบ

- อุปกรณ์ Android ต้องมีการติดตั้งบริการ Google Play

- อุปกรณ์ต้องลงทะเบียนด้วย Intune

สำหรับข้อมูลเพิ่มเติมรวมถึงวิธีการส่งข้อความให้ดูที่[เอกสารประกอบของฟีเจอร์](https://docs.microsoft.com/intune/custom-notifications)
