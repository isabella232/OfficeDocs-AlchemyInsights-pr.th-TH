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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749246"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP บนเครื่อง Linux

คุณสามารถแยกบางไฟล์ โฟลเดอร์ กระบวนการ และไฟล์ที่เปิดประมวลผลจากการสแกน MDATP ได้ การยกเว้นช่วยป้องกันการตรวจหาซอฟต์แวร์และไฟล์ที่ไม่ถูกต้องไม่เฉพาะหรือถูกปรับแต่งให้องค์กรของคุณ การยกเว้นยังช่วยลดปัญหาด้านประสิทธิภาพการคํานวณที่เกิดจาก MDATP อีกด้วย

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517)

> [!IMPORTANT]
> การยกเว้นที่อธิบายในบทความนี้ใช้ไม่ได้กับความสามารถอื่นๆ ของ MDATP for Linux รวมถึงการตรวจหาจุดสิ้นสุดและการตอบกลับ (EDR) ไฟล์ที่คุณแยกออกโดยใช้วิธีที่อธิบายไว้ในบทความนี้ยังคงสามารถทริกเกอร์การแจ้งเตือน EDR และความสามารถในการตรวจจับอื่นๆ ได้
