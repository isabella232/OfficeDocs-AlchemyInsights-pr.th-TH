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
ms.openlocfilehash: 96579b28923e392a0fa05c56833fed1b45eb118437ac7e8333c610ed69126f8e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53916434"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP บนเครื่อง Linux

คุณสามารถแยกบางไฟล์ โฟลเดอร์ กระบวนการ และไฟล์ที่เปิดตามกระบวนการจากการสแกน MDATP ได้ การยกเว้นช่วยป้องกันไม่ให้มีการตรวจหาซอฟต์แวร์และไฟล์ที่ไม่ถูกต้อง ไม่แน่นอน หรือถูกปรับแต่งให้องค์กรของคุณ การยกเว้นยังช่วยบรรเทาปัญหาด้านประสิทธิภาพที่เกิดจาก MDATP

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517)

> [!IMPORTANT]
> การยกเว้นที่อธิบายไว้ในบทความนี้ใช้ไม่ได้กับความสามารถอื่นๆ ของ MDATP for Linux รวมถึงการตรวจหาและการตอบสนองปลายทาง (EDR) ไฟล์ที่คุณแยกออกโดยใช้วิธีที่อธิบายไว้ในบทความนี้ยังคงสามารถทริกเกอร์การแจ้งเตือนEDRและความสามารถในการตรวจสอบอื่นๆ ได้
