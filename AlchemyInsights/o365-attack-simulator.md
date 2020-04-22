---
title: จําลองการโจมตี 2681 ใน Microsoft 365
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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713485"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="e5335-102">จําลองการโจมตีใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e5335-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="e5335-103">คุณหายไปจําลองการโจมตี?</span><span class="sxs-lookup"><span data-stu-id="e5335-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="e5335-104">จําลองการโจมตีจําเป็นต้องมี**แผนการป้องกันภัยคุกคามขั้นสูงของ Office 365 2 (แผน ATP 2)** หรือ**E5 สําหรับองค์กร Office 365**</span><span class="sxs-lookup"><span data-stu-id="e5335-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="e5335-105">จําลองการโจมตี**จะไม่**รวมอยู่ในแผนการป้องกันภัยคุกคามขั้นสูงของ Office 365 1 (แผน ATP 1), Office 365 Enterprise E3 หรือแอป Microsoft 365 สําหรับการสมัครใช้งานทางธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="e5335-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="e5335-106">บัญชีที่คุณใช้เพื่อเปิดการโจมตีแบบจําลองสถานการณ์ต้องการสิทธิ์ผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัยและการตรวจสอบสิทธิ์แบบหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="e5335-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="e5335-107">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกําหนดของตัวจําลองการโจมตี ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)</span><span class="sxs-lookup"><span data-stu-id="e5335-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="e5335-108">สิ่งสําคัญที่ควรทราบเกี่ยวกับการจําลองแบบ**โจมตี Brute Force:**</span><span class="sxs-lookup"><span data-stu-id="e5335-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="e5335-109">หากบัญชีเป้าหมายมีการเปิดใช้งาน MFA และรหัสผ่านถูกเดาอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="e5335-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="e5335-110">แฟ้มรหัสผ่านต้องไม่มากกว่า 10 MB</span><span class="sxs-lookup"><span data-stu-id="e5335-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="e5335-111">ใช้รหัสผ่านหนึ่งต่อบรรทัด และรวมบรรทัดว่าง (carriage return) หลังรหัสผ่านล่าสุดในรายการ</span><span class="sxs-lookup"><span data-stu-id="e5335-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="e5335-112">สิ่งสําคัญที่ควรทราบเกี่ยวกับการจําลองการ**หลอกลวงหอก**แนบ:</span><span class="sxs-lookup"><span data-stu-id="e5335-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="e5335-113">การออกแบบคุณไม่สามารถให้ค่าที่กําหนดเองสําหรับ**URL เซิร์ฟเวอร์การเข้าสู่ระบบฟิชชิ่ง**</span><span class="sxs-lookup"><span data-stu-id="e5335-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="e5335-114">ถ้าผู้รับใช้[Add-in ข้อความรายงาน](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)การเปิดใช้งานเพื่อรายงานข้อความเป็นฟิชชิ่ง คุณอาจไม่ได้รับการแจ้งเตือนสําหรับข้อความ (เนื่องจากนี่เป็นการโจมตีแบบจําลอง)</span><span class="sxs-lookup"><span data-stu-id="e5335-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="e5335-115">รายงาน: หลังจากการโจมตีแบบจําลองสถานการณ์เสร็จสมบูรณ์แล้ว**Attack Details**</span><span class="sxs-lookup"><span data-stu-id="e5335-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="e5335-116">สําหรับคําแนะนําโดยละเอียดและคุณลักษณะใหม่ๆ ใน Simulator การโจมตี ให้ดูที่[เครื่องมือจําลองการโจมตีใน Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="e5335-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
