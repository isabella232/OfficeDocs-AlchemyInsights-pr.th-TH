---
title: กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP บนเครื่อง Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: b2487e283f37498539bfac0583ef7e21d1817db0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321304"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP บนเครื่อง Linux

คุณสามารถยกเว้นบางไฟล์ โฟลเดอร์ กระบวนการ และไฟล์ที่เปิดตามกระบวนการจากการสแกน MDATP การยกเว้นช่วยป้องกันไม่ให้มีการตรวจหาซอฟต์แวร์และไฟล์ที่ไม่ถูกต้อง ไม่แน่นอน หรือถูกปรับแต่งให้องค์กรของคุณ การยกเว้นยังช่วยบรรเทาปัญหาด้านประสิทธิภาพที่เกิดจาก MDATP

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517)

**สิ่ง** สําคัญ: การยกเว้นที่อธิบายไว้ในบทความนี้ใช้ไม่ได้กับความสามารถอื่นๆ ของ MDATP for Linux รวมถึงการตรวจหาและการตอบสนองปลายทาง (EDR) ไฟล์ที่คุณแยกออกโดยใช้วิธีที่อธิบายไว้ในบทความนี้ยังคงสามารถทริกเกอร์การแจ้งเตือนEDRและความสามารถในการตรวจสอบอื่นๆ ได้
