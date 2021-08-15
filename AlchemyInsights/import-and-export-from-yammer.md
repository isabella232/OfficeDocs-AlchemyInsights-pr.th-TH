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
ms.openlocfilehash: 3ead2702c2fbd26b2e5596e26e9189c2f97baf93c93ec3cbd57f15c855b5128e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54001501"
---
# <a name="import-and-export-from-yammer"></a>นําเข้าและส่งออกจากYammer

**นําเข้า**

ตัวเลือกการนําเข้าของผู้ใช้จะแตกต่างกันโดยขึ้นอยู่กับว่าYammerของคุณ[อยู่ในโหมดดั้งเดิม](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)Microsoft 365 หรือไม่

- **โหมดที่ไม่ใช่ภายใน**: ผู้ใช้สามารถนําเข้าไปยังกลุ่มโดยใช้ [เพิ่ม](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) จากสมุดรายชื่อ (จํากัดผู้ใช้สูงสุด 100 ราย) ภายในการตั้งค่ากลุ่ม หรือเครือข่ายโดยใช้ อัปเดตกลุ่มใหญ่ [ภายในผู้ดูแลระบบ](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) เครือข่าย
- **โหมดดั้งเดิม**: ควรดําเนินการเป็นสมาชิกกลุ่มและการเป็นสมาชิกเครือข่ายจากพอร์ทัลผู้ดูแลระบบ [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)พอร์ทัล [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)หรือใช้ตัวเลือก Azure AD อื่น เครือข่ายในโหมดดั้งเดิมไม่สามารถเข้าถึงการอัปเดตแบบเป็นกลุ่มและฟีเจอร์ดั้งเดิมอื่นๆ ได้อีกต่อไป

> [!IMPORTANT]
> Yammerไม่รองรับการนําเข้าเนื้อหาจากภายในผู้ดูแลระบบเครือข่ายแม้ว่าจะใช้ฟีเจอร์การส่งออกข้อมูลในเครือข่ายอื่น เนื้อหาสามารถโพสต์ใหม่ตามโซลูชันของคู่ค้าหรือ API Yammer REST ได้

**ส่งออก**

[ส่งออกข้อมูลเครือข่ายภายในผู้ดูแลระบบ](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data)เครือข่ายจะอนุญาตให้ส่งออกเนื้อหาYammerเครือข่ายของคุณ รวมถึงข้อความและไฟล์ สิ่งที่แนบมาอาจมีขนาดใหญ่มาก และจะทําให้การส่งออกใช้เวลานานในการทําให้เสร็จสมบูรณ์ เราขอแนะให้เครือข่ายที่ใช้งานอยู่ถูกส่งออกโดยใช้ [API การส่งออก](https://developer.yammer.com/docs/data-export-api) ข้อมูลในช่วงตามวันหรือสัปดาห์ ฝ่ายสนับสนุนของ Microsoft ไม่มีสคริปต์แบบปรับแต่งเองเพื่อจุดประสงค์นี้

มี [การส่งออก GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) แยกต่างหากเพื่อส่งออกเนื้อหาของผู้ใช้แต่ละราย