---
title: บันทึกรหัสผ่าน
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
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527777"
---
# <a name="password-logs"></a><span data-ttu-id="c1757-102">บันทึกรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="c1757-102">Password logs</span></span>

<span data-ttu-id="c1757-103">**ฉันมีปัญหาในการเข้าถึงบันทึกการตรวจสอบการตั้งค่ารหัสผ่านใหม่**</span><span class="sxs-lookup"><span data-stu-id="c1757-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="c1757-104">เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการเข้าถึงบันทึกการตรวจสอบการตั้งค่ารหัสผ่านใหม่ ให้ปฏิบัติตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="c1757-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="c1757-105">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดูบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="c1757-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="c1757-106">บทบาทต่อไปนี้ได้รับอนุญาตเท่านั้น:</span><span class="sxs-lookup"><span data-stu-id="c1757-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="c1757-107">ผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="c1757-107">Global administrator</span></span>
 - <span data-ttu-id="c1757-108">ผู้ดูแลระบบความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="c1757-108">Security administrator</span></span>
 - <span data-ttu-id="c1757-109">โปรแกรมอ่านความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="c1757-109">Security reader</span></span>

<span data-ttu-id="c1757-110">**ฉันต้องการดูเหตุการณ์การตรวจสอบการตั้งค่ารหัสผ่านใหม่ทั้งหมดตั้งแต่ที่ฉันปรับใช้ครั้งแรก**</span><span class="sxs-lookup"><span data-stu-id="c1757-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="c1757-111">การรีเซ็ตหรือการลงทะเบียนรหัสผ่านสูงสุด 120,000 รายการจะถูกเก็บไว้ในรายงานของ 30 วันที่ผ่านมา</span><span class="sxs-lookup"><span data-stu-id="c1757-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="c1757-112">ขีดจํากัดสูงสุดนี้ใช้กับ UI เมื่อดาวน์โหลด CSV</span><span class="sxs-lookup"><span data-stu-id="c1757-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="c1757-113">มีเหตุการณ์ 1 ล้านเหตุการณ์ผ่าน PowerShell</span><span class="sxs-lookup"><span data-stu-id="c1757-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="c1757-114">ดูลิงก์ทางด้านล่างเพื่อดูข้อมูลเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="c1757-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="c1757-115">เหตุการณ์การรีเซ็ตรหัสผ่านด้วยตนเองจากรายงาน Azure AD และ API เหตุการณ์</span><span class="sxs-lookup"><span data-stu-id="c1757-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c1757-116">วิธีการดาวน์โหลดเหตุการณ์การลงทะเบียนรีเซ็ตรหัสผ่านอย่างรวดเร็วด้วย PowerShell</span><span class="sxs-lookup"><span data-stu-id="c1757-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="c1757-117">**ฉันต้องการเข้าใจเพิ่มเติมเกี่ยวกับความสามารถในการรายงานการรีเซ็ตรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="c1757-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="c1757-118">ตรวจสอบผู้ที่ลงทะเบียนหรือรีเซ็ตรหัสผ่านด้วยบันทึกการตรวจสอบการรีเซ็ตรหัสผ่าน Azure AD ในพอร์ทัล Azure **ภายใต้ผู้ใช้และ** กลุ่ม</span><span class="sxs-lookup"><span data-stu-id="c1757-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="c1757-119">ดูลิงก์ต่อไปนี้เพื่อดูข้อมูลเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="c1757-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="c1757-120">ภาพรวมรายงานการตั้งค่ารหัสผ่านใหม่</span><span class="sxs-lookup"><span data-stu-id="c1757-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c1757-121">วิธีการดูรายงานรีเซ็ตรหัสผ่านในพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="c1757-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c1757-122">เหตุการณ์การรีเซ็ตรหัสผ่านด้วยตนเองจากรายงาน Azure AD และ API เหตุการณ์</span><span class="sxs-lookup"><span data-stu-id="c1757-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c1757-123">วิธีการดาวน์โหลดเหตุการณ์การลงทะเบียนรีเซ็ตรหัสผ่านอย่างรวดเร็วด้วย PowerShell</span><span class="sxs-lookup"><span data-stu-id="c1757-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


