---
title: รหัสของกฎโพรไฟล์ Provisioning 1029 iOS
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 14d30092-8cf5-4fe6-a2a3-8a337e96cb1c
ms.openlocfilehash: 590dd3d603cfe6581b7dac752ea82df1eab2a141
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29914671"
---
# <a name="ios-provisioning-profiles"></a>โพรไฟล์การเตรียมใช้งาน iOS

เครื่องคอมพิวเตอร์ Apple iOS บรรทัดทางธุรกิจใช้แนวคิดของการเตรียมใช้งานโพรไฟล์ซึ่งใช้ในการตรวจสอบความสมบูรณ์ของแอพลิเคชัน และบังคับใช้นโยบายที่กำหนดไว้ในโพรไฟล์ สิ่งเหล่านี้การเตรียมใช้งานโพรไฟล์หมดอายุหลังจาก 12 เดือน และดังนั้น ต้องเกี่ยวข้องกับโปรแกรมประยุกต์ที่ใช้งานจริงในใบสั่งสำหรับโปรแกรมประยุกต์เพื่อดำเนินต่อเพื่อเรียกใช้ส่วนกำหนดค่าใหม่
  
บทความต่อไปนี้อธิบายวิธีการสร้างการเชื่อมโยงการเตรียมใช้งานใหม่ของโพรไฟล์ ด้วยการ iOS app LOB ที่ปรับใช้ผ่านทาง Intune:[ใช้ iOS app เตรียมใช้งานโพรไฟล์เพื่อป้องกันไม่ให้โปรแกรมประยุกต์ของคุณจากการหมดอายุ](https://docs.microsoft.com/intune/app-provisioning-profile-ios)
  

