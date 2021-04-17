---
title: คะแนนการปฏิบัติตามกฎระเบียบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001483"
- "3519"
ms.openlocfilehash: 78b0658902034560c4f568b1ae2dcd66bb5fb540
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817335"
---
# <a name="compliance-score"></a><span data-ttu-id="b9944-102">คะแนนการปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="b9944-102">Compliance score</span></span>

<span data-ttu-id="b9944-103">คะแนนการปฏิบัติตามนโยบายของ Microsoft (ตัวอย่าง) เป็นฟีเจอร์ใน Microsoft 365 ที่ช่วยให้คุณวัดท่าทางการปฏิบัติตามข้อบังคับขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="b9944-103">Microsoft Compliance Score (Preview) is a feature in Microsoft 365 that helps you measure your organization's compliance posture.</span></span> <span data-ttu-id="b9944-104">ใช้คะแนนตามความเสี่ยงตามความคืบหน้าของการปรับใช้การดําเนินการปฏิบัติตามกฎระเบียบที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="b9944-104">It uses a risk-based score based on your progress of implementing compliance-related actions.</span></span>   <span data-ttu-id="b9944-105">คะแนนการปฏิบัติตามกฎระเบียบเป็นเวอร์ชันที่ง่ายขึ้น [ของตัวจัดการ](https://docs.microsoft.com/microsoft-365/compliance/compliance-manager-overview) การปฏิบัติตามข้อบังคับ และมีวิธีที่ง่ายดายในการตรวจสอบความสอดคล้องของการปฏิบัติตามข้อบังคับของคุณ และใช้การดําเนินการเพื่อปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="b9944-105">Compliance Score is a simplified version of [Compliance Manager](https://docs.microsoft.com/microsoft-365/compliance/compliance-manager-overview) and offers an easier way to examine your compliance stance and implement actions to improve it.</span></span> 

<span data-ttu-id="b9944-106">ผู้ดูแลระบบส่วนกลางจะต้องตั้งค่าสิทธิ์ที่เหมาะสมใน [ศูนย์การปฏิบัติตาม](https://docs.microsoft.com/microsoft-365/security/office-365-security/permissions-in-the-security-and-compliance-center) ข้อบังคับของ Microsoft เพื่อเข้าถึงคะแนนการปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="b9944-106">The Global admin will need to set up the proper [permissions](https://docs.microsoft.com/microsoft-365/security/office-365-security/permissions-in-the-security-and-compliance-center) in the Microsoft Compliance center to access Compliance Score.</span></span>  <span data-ttu-id="b9944-107">สิทธิ์ใดๆ ที่กําหนดค่าไว้ก่อนหน้านี้ให้กับตัวจัดการการปฏิบัติตามกฎระเบียบจะไม่ถ่ายโอนไปยังคะแนนการปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="b9944-107">Any permissions previously configured for Compliance Manager will not transfer to Compliance Score.</span></span>

<span data-ttu-id="b9944-108">**เพื่อเข้าถึงคะแนนการปฏิบัติตามนโยบาย**</span><span class="sxs-lookup"><span data-stu-id="b9944-108">**To access Compliance Score**</span></span>

1. <span data-ttu-id="b9944-109">ไปที่ศูนย์การปฏิบัติตามนโยบายของ Microsoft 365 **และลงชื่อเข้าใช้ด้วย** บัญชีผู้ดูแลระบบส่วนกลางของ Microsoft 365 ของคุณ</span><span class="sxs-lookup"><span data-stu-id="b9944-109">Go to the Microsoft 365 compliance center and **sign in** with your Microsoft 365 global admin account.</span></span>

2. <span data-ttu-id="b9944-110">เลือก **คะแนนการปฏิบัติตาม** นโยบาย บนบานหน้าต่างนําทางด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="b9944-110">Select **Compliance Score** on the left navigation pane.</span></span> <span data-ttu-id="b9944-111">จากนั้นคุณควรจะเห็นแดชบอร์ด [คะแนนการปฏิบัติตามกฎระเบียบที่มีคะแนน](https://docs.microsoft.com/microsoft-365/compliance/compliance-score-setup#understand-the-compliance-score-dashboard)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="b9944-111">You should then see your [Compliance Score dashboard with your score](https://docs.microsoft.com/microsoft-365/compliance/compliance-score-setup#understand-the-compliance-score-dashboard).</span></span>
 

<span data-ttu-id="b9944-112">**ดูข้อมูลเพิ่มเติมเกี่ยวกับ**:</span><span class="sxs-lookup"><span data-stu-id="b9944-112">**For more information on**:</span></span>

- <span data-ttu-id="b9944-113">การตั้งค่าสิทธิ์การเข้าถึงคะแนนการปฏิบัติตามข้อบังคับ ให้ดู [ให้สิทธิ์การเข้าถึงศูนย์การปฏิบัติตามข้อบังคับของ Microsoft 365 แก่](https://docs.microsoft.com/microsoft-365/security/office-365-security/grant-access-to-the-security-and-compliance-center)ผู้ใช้ &การปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="b9944-113">Setting up Access Permissions for Compliance Score, see [Give users access to the Microsoft 365 Security & Compliance Centers](https://docs.microsoft.com/microsoft-365/security/office-365-security/grant-access-to-the-security-and-compliance-center).</span></span>
- <span data-ttu-id="b9944-114">การดาเนินการปรับปรุงในคะแนนการปฏิบัติตามนโยบาย  [ให้ดู การสอดคล้องกับคะแนนการปฏิบัติตาม](https://docs.microsoft.com/microsoft-365/compliance/working-with-compliance-score)นโยบาย</span><span class="sxs-lookup"><span data-stu-id="b9944-114">Working with Improvement Actions in Compliance Score, see  [Working with Compliance Score](https://docs.microsoft.com/microsoft-365/compliance/working-with-compliance-score).</span></span>
- <span data-ttu-id="b9944-115">วิธีการคํานวณคะแนนการปฏิบัติตามกฎระเบียบ ให้ดูที่ [วิธีการคํานวณคะแนนการปฏิบัติตาม](https://docs.microsoft.com/microsoft-365/compliance/compliance-score-methodology)กฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="b9944-115">How Compliance Score is calculated, see [Compliance Score Methodology](https://docs.microsoft.com/microsoft-365/compliance/compliance-score-methodology).</span></span>
- <span data-ttu-id="b9944-116">คะแนนการปฏิบัติตามกฎระเบียบเปรียบเทียบกับตัวจัดการการปฏิบัติตามกฎระเบียบ [ให้ดู ความสัมพันธ์กับตัวจัดการการปฏิบัติตาม](https://docs.microsoft.com/microsoft-365/compliance/compliance-score#relationship-to-compliance-manager)ข้อบังคับ</span><span class="sxs-lookup"><span data-stu-id="b9944-116">Compliance Score vs. Compliance Manager, see [Relationship to Compliance Manager](https://docs.microsoft.com/microsoft-365/compliance/compliance-score#relationship-to-compliance-manager).</span></span>

