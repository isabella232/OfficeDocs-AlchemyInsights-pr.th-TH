---
title: การป้องกันจากการโจมตีจากระบบตีกลับ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037181"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="45b33-102">การป้องกันจากการโจมตีจากระบบตีกลับ</span><span class="sxs-lookup"><span data-stu-id="45b33-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="45b33-103">ระบบตีกลับเป็นรายงานแจ้งการไม่สามารถส่งได้ (หรือที่เรียกว่า NRS หรือข้อความแจ้งการตีกลับ) ที่คุณได้รับจากข้อความที่คุณยังไม่ได้ส่ง</span><span class="sxs-lookup"><span data-stu-id="45b33-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="45b33-104">สแปมเมอร์ปลอมแปลง (ปลอมแปลง) ที่อยู่ **จาก:** ของข้อความของพวกเขา และมักใช้ที่อยู่อีเมลจริงเพื่อให้ข้อความเหล่านั้นมีความน่าเชื่อถือ</span><span class="sxs-lookup"><span data-stu-id="45b33-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="45b33-105">ดังนั้น เมื่อผู้ส่งสแปมส่งข้อความไปยังผู้รับที่ไม่มีอยู่อย่างหลีกเลี่ยงไม่ได้ เซิร์ฟเวอร์อีเมลปลายทางอาจหลอกลวงให้ส่งกลับข้อความที่ไม่สามารถส่งได้ใน NDR ไปยังผู้ส่งที่ปลอมแปลงในที่อยู่ **จาก:**</span><span class="sxs-lookup"><span data-stu-id="45b33-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="45b33-106">ข้อมูลเพิ่มเติมสามารถพบได้ใน[ระบบ Backscatter ใน EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)</span><span class="sxs-lookup"><span data-stu-id="45b33-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="45b33-107">**การเปิดใช้งานการป้องกันระบบป้องกันระบบป้องกันระบบกระทกหลัง**</span><span class="sxs-lookup"><span data-stu-id="45b33-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="45b33-108">เมื่อต้องการเปิดใช้งานการป้องกันระบบกลับ ให้ปฏิบัติตามเส้นทางด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="45b33-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="45b33-109">**protection.office.com > Threat Management > > Antispam > เลือกนโยบายตัวกรองสแปมและแก้ไขนโยบาย > คุณสมบัติสแปม > > การตรวจหาและตีกลับ NDR > ตั้งเป็น "เปิด"**</span><span class="sxs-lookup"><span data-stu-id="45b33-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="45b33-110">ถ้าคุณเชื่อว่าบัญชีถูกละเมิด ให้ดูรายการต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="45b33-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="45b33-111">การตอบสนองต่อบัญชีอีเมลที่ถูกละเมิด</span><span class="sxs-lookup"><span data-stu-id="45b33-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="45b33-112">การเอาผู้ใช้ที่ถูกบล็อกออกจากพอร์ทัลผู้ใช้ที่ถูกบล็อกใน Office 365</span><span class="sxs-lookup"><span data-stu-id="45b33-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



