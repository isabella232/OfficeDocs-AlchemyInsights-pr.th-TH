---
title: ตั้งค่าการจัดการความเสี่ยง Insider
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002284"
- "4405"
ms.openlocfilehash: c4003faac9294725283786fd865217fdc7fcdcef
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446674"
---
# <a name="set-up-insider-risk-management"></a>ตั้งค่าการจัดการความเสี่ยง Insider

เมื่อต้องการเข้าถึงและใช้การจัดการความเสี่ยงจาก Insider องค์กรของคุณต้องมีหนึ่งในการสมัครใช้งานต่อไปนี้:

- Microsoft 365 การสมัครใช้งาน G5 (เวอร์ชันแบบชําระเงินหรือรุ่นทดลองใช้)
- Microsoft 365 G3การสมัครใช้งาน + add-on การปฏิบัติตามMicrosoft 365 G5
- Microsoft 365 G3การสมัครใช้งาน + add-on การจัดการMicrosoft 365 G5 Insider Risk Management
- Office 365 E3การสมัครใช้งาน + Enterprise Mobility and Security E3 + Microsoft 365 E5 Compliance-on

If you don't have an existing Microsoft 365 E5 plan and want to try insider risk management, you can add Microsoft 365 to your existing subscription or sign up for a trial of Microsoft 365 Enterprise E5.

**เคล็ดลับ**:

- การใช้เทมเพลต การรั่วไหลของข้อมูล ตรวจสอบให้แน่ใจว่าคุณได้กําหนดค่านโยบายการป้องกันการสูญหายของข้อมูล (DLP) ไว้อย่างน้อยหนึ่งนโยบาย However, there is a new trigger option that doesn't require a DLP policy to be configured.

- ผู้ดูแลระบบส่วนกลางไม่มีสิทธิ์เข้าถึงพอร์ทัลการจัดการความเสี่ยงจาก Insider ตามค่าเริ่มต้น พวกเขาต้องได้รับมอบหมายบทบาทการจัดการความเสี่ยงจาก Insider

- ถ้าผู้ดูแลระบบไม่เห็นการแจ้งเตือน ให้ตรวจสอบให้แน่ใจว่าผู้ใช้ถูกมอบหมายให้กับกลุ่มใดกลุ่มหนึ่งต่อไปนี้

    นักวิเคราะห์การจัดการความเสี่ยงจาก Insider

    Insider Risk Management Investigators

For more information about how insider risk polices can help you manage risk in your organization, see [Learn about insider risk management in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/insider-risk-management).