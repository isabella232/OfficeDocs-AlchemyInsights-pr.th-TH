---
title: 2681 โจมตีจําลองใน Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506757"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="3bd1c-102">จําลองการโจมตีใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3bd1c-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="3bd1c-103">คุณหายไปโจมตีจําลอง?</span><span class="sxs-lookup"><span data-stu-id="3bd1c-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="3bd1c-104">โปรแกรมจําลองการโจมตีจําเป็นต้องมี**แผนการป้องกันภัยคุกคามขั้นสูง 365 Office 2 (ATP Plan 2)** หรือ**Office 365 Enterprise E5**</span><span class="sxs-lookup"><span data-stu-id="3bd1c-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="3bd1c-105">ตัวจําลองการโจมตี**ไม่ได้**รวมอยู่ในแผนการป้องกันภัยคุกคามขั้นสูงของ Office 365 1 (แผน ATP 1), Office 365 Enterprise E3 หรือแอป Microsoft 365 สําหรับการบอกรับเป็นสมาชิกทางธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="3bd1c-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="3bd1c-106">บัญชีที่คุณใช้เพื่อเปิดใช้การโจมตีจําลองต้องการสิทธิ์ระดับผู้ดูแลหรือผู้ดูแลความปลอดภัยส่วนกลางและการรับรองความถูกต้องด้วยหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="3bd1c-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="3bd1c-107">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกําหนดของ Attack Simulator โปรดดู[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="3bd1c-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="3bd1c-108">สิ่งสําคัญที่ควรรู้เกี่ยวกับ**การจําลองการโจมตี Brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="3bd1c-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="3bd1c-109">หากบัญชีเป้าหมายเปิดใช้งาน MFA และเดารหัสผ่านถูกต้องบัญชีจะไม่แสดงเป็น compromised (ปัจจัยการตรวจสอบที่สองจะไม่สมบูรณ์)</span><span class="sxs-lookup"><span data-stu-id="3bd1c-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="3bd1c-110">แฟ้มรหัสผ่านไม่สามารถมีขนาดใหญ่กว่า 10 เมกะไบต์ได้</span><span class="sxs-lookup"><span data-stu-id="3bd1c-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="3bd1c-111">ใช้รหัสผ่านหนึ่งครั้งต่อบรรทัด และรวมบรรทัดว่าง (กลับค่าขนส่ง) หลังจากรหัสผ่านล่าสุดในรายการ</span><span class="sxs-lookup"><span data-stu-id="3bd1c-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="3bd1c-112">สิ่งสําคัญที่ต้องทราบเกี่ยวกับการจําลอง**การแนบฟิชชิ่ง Spear:**</span><span class="sxs-lookup"><span data-stu-id="3bd1c-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="3bd1c-113">โดยการออกแบบ คุณไม่สามารถกําหนดค่าที่กําหนดเองสําหรับ**URL ของเซิร์ฟเวอร์การเข้าสู่ระบบฟิชชิ่ง**</span><span class="sxs-lookup"><span data-stu-id="3bd1c-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="3bd1c-114">ถ้าผู้รับใช้[add-in การเปิดใช้งานข้อความรายงาน](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)เพื่อรายงานข้อความว่าเป็นฟิชชิ่ง คุณอาจไม่ได้รับข้อความแจ้งเตือน (เนื่องจากเป็นการโจมตีจําลอง)</span><span class="sxs-lookup"><span data-stu-id="3bd1c-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="3bd1c-115">รายงาน: หลังจากการโจมตีจําลองเสร็จสมบูรณ์แล้ว**Attack Details**</span><span class="sxs-lookup"><span data-stu-id="3bd1c-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="3bd1c-116">สําหรับคําแนะนําโดยละเอียดและคุณลักษณะใหม่ในการโจมตีจําลอง ดู[จําลองการโจมตี ใน Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="3bd1c-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
