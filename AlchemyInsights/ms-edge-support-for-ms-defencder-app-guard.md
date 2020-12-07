---
title: การสนับสนุน microsoft Edge สำหรับ Microsoft Defender Guard แอปพลิเคชัน
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584008"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>การสนับสนุน microsoft Edge สำหรับ Microsoft Defender Guard แอปพลิเคชัน

ได้รับการออกแบบมาสำหรับ Windows 10 และ Microsoft Edge, Guard ของแอปพลิเคชันใช้วิธีการแยกฮาร์ดแวร์ที่ช่วยให้ผู้ใช้นำทางไปยังไซต์ที่ไม่น่าเชื่อถือจากภายในที่แยก, Hyper V –เปิดใช้งานคอนเทนเนอร์ที่แยกออกจากระบบปฏิบัติการโฮสต์

ผู้ดูแลระบบขององค์กรจะกำหนดรายการของเว็บไซต์ที่เชื่อถือได้ทรัพยากร cloud และเครือข่ายภายใน เมื่อผู้ใช้เยี่ยมชมไซต์ที่ไม่ได้อยู่ในรายการ Microsoft Edge จะเปิดไซต์ในคอนเทนเนอร์ ซึ่งหมายความว่าถ้าไซต์ดังกล่าวออกมาเป็นอันตรายแล้วพีซีโฮสต์จะยังคงได้รับการป้องกันและผู้โจมตีจะไม่สามารถเข้าถึงข้อมูลขององค์กรได้

การติดตั้งส่วนขยายในคอนเทนเนอร์ได้รับการสนับสนุนจาก Microsoft Edge เวอร์ชัน๘๑และสามารถควบคุมได้ผ่านทางนโยบาย ที่อยู่ updateURL ที่ได้รับการใช้ในนโยบาย ExtensionInstallForcelist ควรถูกเพิ่มเป็นทรัพยากรที่เป็นกลางในนโยบายการแยกเครือข่ายที่ใช้โดย Guard ของแอปพลิเคชัน

สำหรับข้อมูลเพิ่มเติมให้ดูที่[Microsoft Edge สนับสนุนสำหรับ Microsoft Defender Guard แอปพลิเคชัน](https://go.microsoft.com/fwlink/?linkid=2134229)
