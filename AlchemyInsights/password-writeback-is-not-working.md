---
title: Password Writeback ไม่ใช้งาน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243525"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="e94d4-102">Password Writeback ไม่ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e94d4-102">Password Writeback is not working</span></span>

<span data-ttu-id="e94d4-103">**ฉันมีปัญหาในการกําหนดค่า Writeback ของรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="e94d4-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="e94d4-104">Password Writeback เป็นฟีเจอร์ระดับพรีเมียม</span><span class="sxs-lookup"><span data-stu-id="e94d4-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="e94d4-105">ตรวจสอบให้แน่ใจว่าคุณเข้าใจความต้องการด้านสิทธิ์การใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="e94d4-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="e94d4-106">คุณต้องมีอย่างน้อยหนึ่งสิทธิ์การใช้งานที่มอบหมายในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="e94d4-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="e94d4-107">**ระบบคลาวด์เฉพาะผู้ใช้** - Office 365 (O365) ชําระเงิน SKU หรือ Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="e94d4-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="e94d4-108">**ผู้ใช้ระบบคลาวด์และ/หรือผู้ใช้ในองค์กร** - Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="e94d4-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="e94d4-109">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับข้อตามความต้องการด้านสิทธิ์การใช้งาน ให้ดู [ข้อกฎหมายการให้สิทธิ์การใช้งานรีเซ็ตรหัสผ่านด้วยตนเองของ Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="e94d4-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="e94d4-110">คุณมีบัญชีผู้ดูแลระบบอย่างน้อยหนึ่งบัญชีและบัญชีผู้ใช้ทดสอบหนึ่งบัญชีที่มีหนึ่งในสิทธิ์การใช้งานที่เหมาะสม</span><span class="sxs-lookup"><span data-stu-id="e94d4-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="e94d4-111">คุณต้องเชื่อมต่อ Azure AD Connect กับตัว Emulator ของตัวควบคุมโดเมนหลักเพื่อให้สามารถใช้งานการเขียนรหัสผ่านได้</span><span class="sxs-lookup"><span data-stu-id="e94d4-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="e94d4-112">คุณสามารถกําหนดค่า Azure AD Connect ให้ใช้ตัวควบคุมโดเมนหลักโดยคลิกขวาที่คุณสมบัติของตัวเชื่อมต่อการซิงโครไนซ์ Active Directory แล้วเลือก **กําหนดค่าพาร์ติชัน** ไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="e94d4-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="e94d4-113">จากที่นั่น ให้ค้นหา **ส่วนการตั้งค่าการเชื่อมต่อ** ตัวควบคุมโดเมน และตรวจสอบกล่องที่มีชื่อเรื่อง **ว่าใช้ตัวควบคุมโดเมนที่ต้องการ** เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="e94d4-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="e94d4-114">ถ้า DC ที่ต้องการไม่ใช่ตัวเลียนแบบ PDC Azure AD Connect จะยังคงติดต่อไปยัง PDC เพื่อเขียนรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="e94d4-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="e94d4-115">การกําหนดค่าและเปิดใช้งานการตั้งค่ารหัสผ่านใหม่ในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="e94d4-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="e94d4-116">หากต้องการข้อมูลเพิ่มเติม โปรดดู [การเปิดใช้งานผู้ใช้เพื่อตั้งค่ารหัสผ่าน Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)ใหม่</span><span class="sxs-lookup"><span data-stu-id="e94d4-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="e94d4-117">ตรวจสอบให้แน่ใจว่าบัญชีผู้ดูแลระบบที่ใช้เพื่อเปิดใช้งาน Password Writeback เป็นบัญชีผู้ดูแลระบบระบบคลาวด์ (ที่สร้างใน Azure AD ไม่ใช่ AD ภายในองค์กร)</span><span class="sxs-lookup"><span data-stu-id="e94d4-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="e94d4-118">คุณมีการปรับใช้แบบภายในองค์กรแบบหลายฟอเรสต์หรือหลายฟอเรสต์ที่ใช้งาน Windows Server 2008 R2, Windows Server 2012 หรือ Windows Server 2012 R2 ที่มี Service Pack ล่าสุดติดตั้งอยู่</span><span class="sxs-lookup"><span data-stu-id="e94d4-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="e94d4-119">คุณได้ติดตั้งเครื่องมือ Azure AD Connect และได้จัดเตรียมสภาพแวดล้อม AD ของคุณไว้เพื่อซิงโครไนซ์กับระบบคลาวด์</span><span class="sxs-lookup"><span data-stu-id="e94d4-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="e94d4-120">ก่อนที่จะทดสอบ Writeback ของรหัสผ่าน ตรวจสอบให้แน่ใจว่าคุณเสร็จสิ้นการนําเข้าและการซิงค์แบบเต็มจากทั้ง AD และ Azure AD ใน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e94d4-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="e94d4-121">เมื่อต้องการเรียนรู้เพิ่มเติม ดูวิธีการซิงค์แบบเต็ม [และนําเข้าแบบเต็มใน Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="e94d4-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="e94d4-122">**ฉันมีปัญหากับการเชื่อมต่อ Writeback ของรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="e94d4-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="e94d4-123">ดาวน์โหลดและเปิดใช้งาน [Azure AD Connect เวอร์ชันล่าสุด](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="e94d4-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="e94d4-124">การกําหนดค่าไฟร์วอลล์: เครื่องมือ Azure AD Connect (1.1.443 ขึ้นไป) จะต้อง **มีสิทธิ์การเข้าถึง HTTPS** ขาออก:</span><span class="sxs-lookup"><span data-stu-id="e94d4-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="e94d4-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e94d4-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="e94d4-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="e94d4-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="e94d4-127">อนุญาตให้การเชื่อมต่อที่ไม่ได้ใช้งานยังคงอยู่เป็นเวลาอย่างน้อย 2-3 นาที</span><span class="sxs-lookup"><span data-stu-id="e94d4-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="e94d4-128">**ฉันยังคงมีปัญหากับ Writeback รหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="e94d4-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="e94d4-129">ถ้าคุณยังพบปัญหา ให้ลองปิดใช้งานและเปิดใช้งานบริการ Writeback ของรหัสผ่านอีกครั้งในเครื่องมือ Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e94d4-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="e94d4-130">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดูวิธีการปิดใช้งาน [และเปิดใช้งาน Writeback รหัสผ่านอีกครั้ง](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="e94d4-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
