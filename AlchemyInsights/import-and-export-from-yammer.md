---
title: นําเข้าและส่งออกจาก Yammer
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
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037256"
---
# <a name="import-and-export-from-yammer"></a>นําเข้าและส่งออกจาก Yammer

**นําเข้า**

ตัวเลือกการนําเข้าของผู้ใช้จะแตกต่างกันโดยขึ้นอยู่กับว่าเครือข่าย Yammer ของคุณ [อยู่ในโหมดดั้งเดิมของ Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)หรือไม่

- **โหมดที่ไม่ใช่โหมด** ดั้งเดิม: ผู้ใช้สามารถนําเข้าไปยังกลุ่มโดยใช้ [เพิ่ม](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) จากสมุดรายชื่อ (จํากัดให้ผู้ใช้ 100 ราย) ภายในการตั้งค่ากลุ่ม หรือเครือข่ายโดยใช้ อัปเดตเป็นกลุ่ม [ภายในผู้ดูแลระบบ](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) เครือข่าย
- **โหมดดั้งเดิม**: การเป็นสมาชิกกลุ่มและการดําเนินการเป็นสมาชิกเครือข่ายควรดําเนินการจากพอร์ทัลผู้ดูแลระบบ [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)พอร์ทัล [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)หรือใช้ตัวเลือก Azure AD อื่น เครือข่ายในโหมดดั้งเดิมจะไม่มีสิทธิ์เข้าถึงการอัปเดตเป็นกลุ่มและฟีเจอร์ดั้งเดิมอื่นๆ อีกต่อไป

> [!IMPORTANT]
> Yammer ไม่สนับสนุนการนําเข้าเนื้อหาจากภายในผู้ดูแลระบบเครือข่าย แม้ว่าจะมีการใช้งานฟีเจอร์การส่งออกข้อมูลในเครือข่ายอื่น เนื้อหาสามารถโพสต์ใหม่ได้โดยโซลูชันของคู่ค้าหรือ API ของ Yammer REST

**ส่งออก**

[ส่งออกข้อมูลเครือข่ายภายในผู้ดูแลระบบ](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) เครือข่ายอนุญาตให้ส่งออกเนื้อหาจากเครือข่าย Yammer รวมถึงข้อความและไฟล์ สิ่งที่แนบมาอาจมีขนาดใหญ่มาก และจะทําให้การส่งออกใช้เวลานานในการทําให้เสร็จสมบูรณ์ เราขอแนะให้เครือข่ายที่ใช้งานอยู่ถูกส่งออกโดยใช้ [API การส่งออก](https://developer.yammer.com/docs/data-export-api) ข้อมูลในช่วงตามวันหรือสัปดาห์ ฝ่ายสนับสนุนของ Microsoft ไม่มีสคริปต์แบบปรับแต่งเองเพื่อวัตถุประสงค์นี้

มี [การส่งออก GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) แยกต่างหากเพื่อส่งออกเนื้อหาให้กับผู้ใช้แต่ละราย