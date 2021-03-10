---
title: ตัวอย่างนโยบายการป้องกันฟิชชิ่งของ Microsoft Defender for Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695639"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="cfb68-102">ตัวอย่างนโยบายการป้องกันฟิชชิ่งของ Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="cfb68-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="cfb68-103">การตั้งค่าเหล่านี้จะเปิดใช้งานนโยบายที่เรียกว่า *โดเมนและ CEO*</span><span class="sxs-lookup"><span data-stu-id="cfb68-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="cfb68-104">นโยบายนี้จะมีทั้งการป้องกันผู้ใช้และโดเมนจากการเลียนแบบ จากนั้นจะปรับใช้นโยบายกับอีเมลทั้งหมดที่ได้รับโดยผู้ใช้ภายในโดเมน</span><span class="sxs-lookup"><span data-stu-id="cfb68-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="cfb68-105">ก่อนอื่น ให้เพิ่มข้อมูลต่อไปนี้เพื่อสร้างนโยบาย:</span><span class="sxs-lookup"><span data-stu-id="cfb68-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="cfb68-106">**ชื่อ**: ข้อความเกี่ยวกับ **โดเมนและ** ประธานเจ้าหน้าที่บริหาร : ตรวจสอบให้แน่ใจว่า CEO และโดเมนของคุณไม่ได้เลียนแบบ</span><span class="sxs-lookup"><span data-stu-id="cfb68-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="cfb68-107">**ใช้กับ**: **เลือกโดเมนผู้รับ** คือ</span><span class="sxs-lookup"><span data-stu-id="cfb68-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="cfb68-108">**ภายใต้ ตัวเลือก** เหล่านี้ **ให้เลือก** เลือก แล้วเลือกโดเมน</span><span class="sxs-lookup"><span data-stu-id="cfb68-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="cfb68-109">เลือก **+** เพิ่ม</span><span class="sxs-lookup"><span data-stu-id="cfb68-109">Select **+ Add**.</span></span> <span data-ttu-id="cfb68-110">เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากชื่อของโดเมนในรายการ (ตัวอย่างเช่น contoso.com )**แล้วเลือก** เพิ่ม</span><span class="sxs-lookup"><span data-stu-id="cfb68-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="cfb68-111">เลือกเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="cfb68-111">Select **Done**.</span></span>
- <span data-ttu-id="cfb68-112">หลังจากสร้างนโยบายแล้ว คุณสามารถปรับแต่งนโยบายโดยใช้ตัวเลือกต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="cfb68-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="cfb68-113">**เพิ่มผู้ใช้เพื่อป้องกัน:** ในตัวอย่างนี้ ให้เพิ่มอีเมลแอดเดรสของ CEO เป็นอย่างน้อย</span><span class="sxs-lookup"><span data-stu-id="cfb68-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="cfb68-114">**เพิ่มโดเมนเพื่อป้องกัน**: เพิ่มโดเมนขององค์กรที่มีสํานักงานของ CEO</span><span class="sxs-lookup"><span data-stu-id="cfb68-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="cfb68-115">**เลือก การ** แอคชัน **:** ถ้าอีเมลถูกส่งโดยผู้ใช้ที่เลียนแบบ ให้เลือก เปลี่ยนเส้นทางข้อความไปยังที่อยู่อีเมลอื่น แล้วใส่ที่อยู่อีเมลของผู้ดูแลระบบความปลอดภัย (ตัวอย่างเช่น *securityadmin@contoso.com)*</span><span class="sxs-lookup"><span data-stu-id="cfb68-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="cfb68-116">ถ้า **อีเมลถูกส่งโดยโดเมนที่เลียนแบบ ให้เลือก\*\*\*\*กักกัน** ข้อความ</span><span class="sxs-lookup"><span data-stu-id="cfb68-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="cfb68-117">**ข่าวกรอง** กล่องจดหมาย: ตามค่าเริ่มต้น ตัวเลือกนี้จะถูกเลือกเมื่อคุณสร้างนโยบายการป้องกันการฟิชชิ่งใหม่</span><span class="sxs-lookup"><span data-stu-id="cfb68-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="cfb68-118">เปิดการตั้งค่า **นี้** ทิ้งไว้เพื่อให้ได้ผลลัพธ์ที่ดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="cfb68-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="cfb68-119">**เพิ่มผู้ส่งและโดเมนที่เชื่อถือได้:** ตัวอย่างเช่น อย่ากําหนดการแทนที่ใดๆ</span><span class="sxs-lookup"><span data-stu-id="cfb68-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="cfb68-120">เมื่อคุณตรวจสอบการตั้งค่าของคุณแล้ว ให้เลือก **สร้างนโยบาย** นี้ **หรือ** บันทึกตามความเหมาะสม</span><span class="sxs-lookup"><span data-stu-id="cfb68-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="cfb68-121">เมื่อต้องการเรียนรู้เพิ่มเติม ดู[นโยบายการป้องกันฟิชชิ่งใน Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="cfb68-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
