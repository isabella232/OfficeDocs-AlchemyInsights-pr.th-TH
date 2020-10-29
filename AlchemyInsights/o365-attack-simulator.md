---
title: ๒๖๘๑จำลองการโจมตีใน Microsoft ๓๖๕
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801570"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="33e77-102">จำลองการโจมตีใน Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="33e77-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="33e77-103">คุณไม่พบการจำลองการโจมตีใช่ไหม</span><span class="sxs-lookup"><span data-stu-id="33e77-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="33e77-104">จำลองการโจมตีจำเป็นต้องมี **Microsoft Defender สำหรับ Office ๓๖๕ Plan 2 (ATP plan 2)** หรือ **Office ๓๖๕ Enterprise E5**</span><span class="sxs-lookup"><span data-stu-id="33e77-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="33e77-105">การโจมตี Simulator **ไม่รวมอยู่** ใน Microsoft Defender สำหรับ Office ๓๖๕ Plan 1 (ATP Plan 1), Office ๓๖๕ Enterprise E3 หรือแอป Microsoft ๓๖๕สำหรับการสมัครใช้งานทางธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="33e77-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="33e77-106">บัญชีผู้ใช้ที่คุณใช้เพื่อเปิดใช้งานการโจมตีแบบจำลองจำเป็นต้องมีสิทธิ์ผู้ดูแลระบบส่วนกลางหรือสิทธิ์ผู้ดูแลระบบความปลอดภัยและการรับรองความถูกต้องแบบหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="33e77-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="33e77-107">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับความต้องการของการโจมตีของ Simulator ให้ดู[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="33e77-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="33e77-108">สิ่งสำคัญที่ควรทราบเกี่ยวกับการจำลองการโจมตีของ **รหัสผ่าน** ที่รุนแรง:</span><span class="sxs-lookup"><span data-stu-id="33e77-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="33e77-109">ถ้าบัญชีผู้ใช้เป้าหมายมีการเปิดใช้งาน MFA และรหัสผ่านถูกคาดเดาได้อย่างถูกต้องบัญชีผู้ใช้จะไม่แสดงเป็นที่ถูกบุกรุก (ปัจจัยการรับรองความถูกต้องที่สองจะไม่สมบูรณ์)</span><span class="sxs-lookup"><span data-stu-id="33e77-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="33e77-110">ไฟล์รหัสผ่านจะต้องมีขนาดใหญ่กว่า10เมกะไบต์</span><span class="sxs-lookup"><span data-stu-id="33e77-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="33e77-111">ใช้รหัสผ่านหนึ่งบรรทัดต่อหนึ่งบรรทัดและรวมบรรทัดว่าง (ส่งกลับค่าขนส่ง) หลังจากรหัสผ่านสุดท้ายในรายการ</span><span class="sxs-lookup"><span data-stu-id="33e77-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="33e77-112">สิ่งสำคัญที่ควรทราบเกี่ยวกับสถานการณ์จำลองที่แนบมาของการ **ฟิชชิ่งของหอก** :</span><span class="sxs-lookup"><span data-stu-id="33e77-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="33e77-113">ตามการออกแบบคุณจะไม่สามารถใส่ค่าที่กำหนดเองสำหรับ **URL ของเซิร์ฟเวอร์การเข้าสู่ระบบฟิชชิ่ง** ได้</span><span class="sxs-lookup"><span data-stu-id="33e77-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="33e77-114">ถ้าผู้รับใช้ [Add-in ข้อความรายงาน](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) เพื่อรายงานข้อความเป็นฟิชชิ่งคุณอาจไม่ได้รับการแจ้งเตือนสำหรับข้อความ (เนื่องจากเป็นการโจมตีแบบจำลอง)</span><span class="sxs-lookup"><span data-stu-id="33e77-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="33e77-115">รายงาน: หลังจากการโจมตีแบบจำลองเสร็จสมบูรณ์แล้วคุณสามารถคลิก **รายละเอียดการโจมตี** เพื่อดูรายงานได้</span><span class="sxs-lookup"><span data-stu-id="33e77-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="33e77-116">สำหรับคำแนะนำโดยละเอียดและฟีเจอร์ใหม่ในการโจมตีจำลองให้ดู[ที่จำลองการโจมตีใน Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="33e77-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
