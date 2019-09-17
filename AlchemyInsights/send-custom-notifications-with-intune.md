---
title: ส่งการแจ้งเตือนที่กำหนดเองด้วย Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992331"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>วิธีการส่งการแจ้งเตือนที่กำหนดเองไปยังผู้ใช้ของอุปกรณ์ iOS และ Android ที่มีการจัดการ

การแจ้งเตือนแบบกำหนดเองสำหรับ Intune จะถูกประมวลผลโดยแอพลิเคชันพอร์ทัลของบริษัทบนอุปกรณ์ของผู้ใช้ การตรวจสอบแล้วสร้างการแจ้งเตือนผลักดันบนอุปกรณ์ที่

ต่อไปนี้เป็นข้อกำหนดเบื้องต้นของอุปกรณ์เพื่อสนับสนุนการรับการแจ้งเตือนที่กำหนดเองและสำหรับแอปเพื่อสร้างการแจ้งเตือนแบบพุช:

- อุปกรณ์ต้องมีการติดตั้งแอพ Portal ของบริษัท  

- อุปกรณ์ต้องอนุญาตให้แอพลิเคชันพอร์ทัลของบริษัทส่งการแจ้งเตือนแบบพุช เมื่อมีการติดตั้งหรือปรับปรุงแอปพลิเคชันจะพร้อมท์ให้ผู้ใช้อนุญาตการแจ้งเตือน

- อุปกรณ์ Android จะต้องมีการติดตั้งบริการ Google Play

- อุปกรณ์ต้องลงทะเบียนกับ Intune

สำหรับข้อมูลเพิ่มเติมรวมถึงวิธีการส่งข้อความให้ดูที่[เอกสารคุณลักษณะ](https://docs.microsoft.com/intune/custom-notifications)
