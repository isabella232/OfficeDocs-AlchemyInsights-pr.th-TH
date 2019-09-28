---
title: ๒๖๘๑โจมตีจำลองใน Office ๓๖๕
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305350"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="7493b-102">จำลองการโจมตีใน Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="7493b-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="7493b-103">คุณขาดการโจมตีจำลอง?</span><span class="sxs-lookup"><span data-stu-id="7493b-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="7493b-104">จำลองการโจมตีต้องใช้**Office ๓๖๕ขั้นสูงป้องกันภัยคุกคามแผน 2 (ATP แผน 2)** หรือ**Office ๓๖๕องค์กร E5**</span><span class="sxs-lookup"><span data-stu-id="7493b-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="7493b-105">โจมตีจำลอง**ไม่ได้**รวมอยู่ใน Office ๓๖๕การป้องกันภัยคุกคามขั้นสูงแผน 1 (ATP แผน 1), Office ๓๖๕องค์กร E3 หรือใดๆ office ๓๖๕การบอกรับเป็นสมาชิกธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="7493b-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="7493b-106">บัญชีที่คุณใช้ในการเปิดการโจมตีจำลองจำเป็นต้องมีผู้ดูแลระบบส่วนกลางหรือสิทธิ์ของผู้ดูแลความปลอดภัยและการรับรองความถูกต้องด้วยหลายปัจจัย (MFA)</span><span class="sxs-lookup"><span data-stu-id="7493b-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="7493b-107">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกำหนดในการโจมตีจำลองโปรดดู[หัวข้อนี้](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)</span><span class="sxs-lookup"><span data-stu-id="7493b-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="7493b-108">สิ่งสำคัญที่ควรรู้เกี่ยวกับการจำลองการโจมตีด้วย**รหัสผ่านที่โง่แรง**:</span><span class="sxs-lookup"><span data-stu-id="7493b-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="7493b-109">หากบัญชีเป้าหมายมี MFA เปิดใช้งานและรหัสผ่านถูกคาดเดาอย่างถูกต้องบัญชีจะไม่แสดงเป็นอันตราย (ปัจจัยการรับรองความถูกต้องที่สองจะไม่สมบูรณ์)</span><span class="sxs-lookup"><span data-stu-id="7493b-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="7493b-110">แฟ้มรหัสผ่านไม่สามารถมีขนาดใหญ่กว่า10เมกะไบต์</span><span class="sxs-lookup"><span data-stu-id="7493b-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="7493b-111">ใช้รหัสผ่านหนึ่งรายการต่อบรรทัดและรวมบรรทัดว่าง (การส่งคืนค่าขนย้าย) หลังจากรหัสผ่านล่าสุดในรายการ</span><span class="sxs-lookup"><span data-stu-id="7493b-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="7493b-112">สิ่งสำคัญที่ควรรู้เกี่ยวกับหอกแนบการ**ฟิชชิ่ง**:</span><span class="sxs-lookup"><span data-stu-id="7493b-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="7493b-113">โดยการออกแบบคุณไม่สามารถระบุค่าที่กำหนดเองสำหรับ**URL ของเซิร์ฟเวอร์การเข้าสู่ระบบแบบฟิชชิ่ง**ได้</span><span class="sxs-lookup"><span data-stu-id="7493b-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="7493b-114">ถ้าผู้รับใช้[เปิดใช้งานข้อความรายงาน add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)เพื่อรายงานข้อความว่าเป็นฟิชชิ่งคุณอาจไม่ได้รับการแจ้งเตือนสำหรับข้อความ (เนื่องจากเป็นการโจมตีแบบจำลอง)</span><span class="sxs-lookup"><span data-stu-id="7493b-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="7493b-115">รายงาน: หลังจากการโจมตีที่จำลองเสร็จสมบูรณ์แล้วคุณสามางานคลิกราย**ละเอียดการโจมตี**เพื่อดูรายงาน</span><span class="sxs-lookup"><span data-stu-id="7493b-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="7493b-116">สำหรับคำแนะนำโดยละเอียดและคุณลักษณะใหม่ในการโจมตีจำลองดูการ[โจมตีจำลองใน Office ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="7493b-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
