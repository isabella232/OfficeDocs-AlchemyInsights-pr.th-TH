---
title: 2681 Attack In Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545745"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="c0fcc-102">Attack In Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c0fcc-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="c0fcc-103">คุณพลาด Attack 11 ใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="c0fcc-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="c0fcc-104">Attack Defender ต้องใช้ **Microsoft Defender Office 365 Plan 2** หรือ Office 365 Enterprise **E5**</span><span class="sxs-lookup"><span data-stu-id="c0fcc-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="c0fcc-105">Attack Defender **จะไม่** รวมอยู่ใน Microsoft Defender Office 365 Plan 1, Office 365 Enterprise E3 หรือMicrosoft 365 Apps for businessอื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="c0fcc-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="c0fcc-106">บัญชีที่คุณใช้เพื่อเปิดใช้การโจมตีที่จําเป็นต้องมีผู้ดูแลระบบส่วนกลางหรือสิทธิ์ของผู้ดูแลระบบความปลอดภัยและการรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="c0fcc-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="c0fcc-107">For more information about Attack Attack Attack requirements, [see this](/microsoft-365/security/office-365-security/attack-simulator)topic .</span><span class="sxs-lookup"><span data-stu-id="c0fcc-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="c0fcc-108">สิ่งสําคัญที่ควรทราบ **เกี่ยวกับสถานการณ์โจมตีของ Brute Force** Password:</span><span class="sxs-lookup"><span data-stu-id="c0fcc-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="c0fcc-109">ถ้าบัญชีเป้าหมายเปิดใช้งาน MFA และรหัสผ่านคาดเดาไม่ถูกต้อง บัญชีจะไม่แสดงเป็นบัญชีที่ถูกละเมิด (ปัจจัยการรับรองความถูกต้องที่สองจะไม่สมบูรณ์)</span><span class="sxs-lookup"><span data-stu-id="c0fcc-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="c0fcc-110">ไฟล์รหัสผ่านไม่สามารถมีขนาดใหญ่กว่า 10 MB ได้</span><span class="sxs-lookup"><span data-stu-id="c0fcc-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="c0fcc-111">ใช้รหัสผ่านหนึ่งรหัสผ่านต่อบรรทัด และใส่บรรทัดว่าง (อักขระขึ้นบรรทัดใหม่) หลังรหัสผ่านสุดท้ายในรายการ</span><span class="sxs-lookup"><span data-stu-id="c0fcc-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="c0fcc-112">สิ่งสําคัญที่ควรทราบ **เกี่ยวกับฟิชชิ่งของ Phishing** แนบการสถานการณ์:</span><span class="sxs-lookup"><span data-stu-id="c0fcc-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="c0fcc-113">ตามการออกแบบ คุณไม่สามารถใส่ URL ของเซิร์ฟเวอร์การเข้าสู่ระบบฟิชชิ่ง</span><span class="sxs-lookup"><span data-stu-id="c0fcc-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="c0fcc-114">ถ้าผู้รับใช้ [Add-in เปิดใช้งานข้อความ](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) รายงาน เพื่อรายงานข้อความเป็นฟิชชิ่ง คุณอาจไม่ได้รับการแจ้งเตือนข้อความนั้น (เนื่องจากนี่คือการโจมตีที่จําเป็น)</span><span class="sxs-lookup"><span data-stu-id="c0fcc-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="c0fcc-115">รายงาน: หลังจากการโจมตีที่จําเป็นเสร็จสมบูรณ์ คุณสามารถ **คลิก รายละเอียด** การโจมตี เพื่อดูรายงานได้</span><span class="sxs-lookup"><span data-stu-id="c0fcc-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="c0fcc-116">ดูคําแนะนําโดยละเอียดและฟีเจอร์ใหม่ใน Attackขออภัย[ให้ดู Attackขออภัยใน Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="c0fcc-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
