---
title: นําเข้าและส่งออกจากYammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: b365921d3ca64e8ad4bd3891e11add8043b2a903
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329845"
---
# <a name="import-and-export-from-yammer"></a>นําเข้าและส่งออกจากYammer

**นําเข้า**

ตัวเลือกการนําเข้าของผู้ใช้จะแตกต่างกันโดยขึ้นอยู่กับว่าYammerของคุณ[อยู่ในโหมดดั้งเดิม](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)Microsoft 365 หรือไม่

- **โหมดที่ไม่ใช่โหมด** ดั้งเดิม: ผู้ใช้สามารถนําเข้าไปยังกลุ่มโดยใช้ [เพิ่ม](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) จากสมุดรายชื่อ (จํากัดผู้ใช้สูงสุด 100 ราย) ภายในการตั้งค่ากลุ่ม หรือไปยังเครือข่ายโดยใช้ อัปเดตกลุ่มใหญ่ [ภายในผู้ดูแลระบบ](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) เครือข่าย
- **โหมดดั้งเดิม**: ควรดําเนินการเป็นสมาชิกกลุ่มและการเป็นสมาชิกเครือข่ายจากพอร์ทัลผู้ดูแลระบบ [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)พอร์ทัล Azure [AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)หรือใช้ตัวเลือก Azure AD อื่น เครือข่ายในโหมดดั้งเดิมไม่สามารถเข้าถึงการอัปเดตแบบเป็นกลุ่มและฟีเจอร์ดั้งเดิมอื่นๆ ได้อีกต่อไป

    **สิ่ง** สําคัญ: Yammerนําเข้าเนื้อหาจากภายในผู้ดูแลระบบเครือข่ายไม่ได้รับการสนับสนุน แม้ว่าจะมีการใช้ฟีเจอร์การส่งออกข้อมูลในเครือข่ายอื่น เนื้อหาสามารถโพสต์ใหม่ได้โดยโซลูชันของคู่ค้าหรือ API Yammer REST

**ส่งออก**

[ส่งออกข้อมูลเครือข่ายภายในผู้ดูแลระบบ](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data)เครือข่ายจะอนุญาตให้ส่งออกเนื้อหาYammerเครือข่ายของคุณ รวมถึงข้อความและไฟล์ สิ่งที่แนบมาอาจมีขนาดใหญ่มาก และจะทําให้การส่งออกใช้เวลานานในการทําให้เสร็จสิ้น เราขอแนะให้เครือข่ายที่ใช้งานอยู่ถูกส่งออกโดยใช้ [API การส่งออก](https://developer.yammer.com/docs/data-export-api) ข้อมูลในช่วงตามวันหรือสัปดาห์ ฝ่ายสนับสนุนของ Microsoft ไม่มีสคริปต์แบบปรับแต่งเองเพื่อจุดประสงค์นี้

มี [การส่งออก GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) แยกต่างหากเพื่อส่งออกเนื้อหาของผู้ใช้แต่ละราย