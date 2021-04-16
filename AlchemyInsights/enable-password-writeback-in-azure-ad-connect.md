---
title: เปิดใช้งานการเขียนกลับรหัสผ่านใน Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814031"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="7ae1b-102">เปิดใช้งานการเขียนกลับรหัสผ่านใน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="7ae1b-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="7ae1b-103">เมื่อต้องการเปิดใช้งาน Writeback รีเซ็ตรหัสผ่านแบบบริการตนเอง ก่อนอื่น ให้เปิดใช้งานตัวเลือกการเขียนกลับใน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="7ae1b-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="7ae1b-104">จากเซิร์ฟเวอร์ Azure AD Connect ของคุณ ให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7ae1b-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="7ae1b-105">ลงชื่อเข้าใช้เซิร์ฟเวอร์ Azure AD Connect ของคุณ และเริ่มตัวช่วยสร้างการ **กําหนดค่า Azure AD Connect**</span><span class="sxs-lookup"><span data-stu-id="7ae1b-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="7ae1b-106">บนหน้า **ยินดีต้อนรับ** ให้คลิก **กําหนด** ค่า</span><span class="sxs-lookup"><span data-stu-id="7ae1b-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="7ae1b-107">บนหน้า **งานเพิ่มเติม** ให้เลือก **ปรับแต่งตัวเลือก** การซิงโครไนซ์ **แล้วคลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="7ae1b-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="7ae1b-108">บนหน้า **เชื่อมต่อไปยัง Azure AD** ให้ใส่ข้อมูลรับรองความถูกต้องของผู้ดูแลระบบส่วนกลางของผู้เช่า Azure ของคุณ **แล้วคลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="7ae1b-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="7ae1b-109">บนหน้า **เชื่อมต่อไดเรกทอรี** และ **การกรอง Domain/OU** **ให้คลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="7ae1b-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="7ae1b-110">บนหน้า **ฟีเจอร์เพิ่มเติม** ให้เลือกกล่องที่อยู่ถัดจาก รหัสผ่าน **การเขียนกลับ\*\*\*\*แล้วคลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="7ae1b-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="7ae1b-111">บนหน้า **พร้อมที่จะกําหนดค่า** ให้คลิก **กําหนดค่า** และรอให้กระบวนการเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="7ae1b-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="7ae1b-112">เมื่อคุณเห็นการกําหนดค่าเสร็จสิ้น **ให้คลิก** ออก</span><span class="sxs-lookup"><span data-stu-id="7ae1b-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="7ae1b-113">เมื่อเปิดใช้งานการเขียนกลับรหัสผ่านใน Azure AD Connect ให้กําหนดค่า Azure AD SSPR เป็น writeback</span><span class="sxs-lookup"><span data-stu-id="7ae1b-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="7ae1b-114">เมื่อต้องการเปิดใช้งานการเขียนกลับของรหัสผ่านใน SSPR ให้เสร็จสิ้นขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7ae1b-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="7ae1b-115">ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้บัญชีผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="7ae1b-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="7ae1b-116">ค้นหาและเลือก **Azure Active Directory\*\*\*\*คลิก รีเซ็ต** รหัสผ่าน **จากนั้นคลิก การรวมภายใน** องค์กร</span><span class="sxs-lookup"><span data-stu-id="7ae1b-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="7ae1b-117">ตั้งค่าตัวเลือกให้ **เขียนรหัสผ่านกลับลงในไดเรกทอรีภายในองค์กรของคุณใช่ไหม\*\*\*\*เป็น** ใช่</span><span class="sxs-lookup"><span data-stu-id="7ae1b-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="7ae1b-118">ตั้งค่าตัวเลือกให้ **อนุญาตให้ผู้ใช้ปลดล็อกบัญชีโดยไม่ต้องรีเซ็ตรหัสผ่านของพวกเขา\*\*\*\*ใช่หรือไม่ เป็น** ใช่</span><span class="sxs-lookup"><span data-stu-id="7ae1b-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="7ae1b-119">เมื่อพร้อม **ให้คลิก** บันทึก</span><span class="sxs-lookup"><span data-stu-id="7ae1b-119">When ready, click **Save**.</span></span>

<span data-ttu-id="7ae1b-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="7ae1b-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="7ae1b-121">เมื่อผู้ดูแลระบบรีเซ็ตรหัสผ่านของผู้ใช้ในพอร์ทัล Azure ถ้าผู้ใช้รายนั้นติดต่อกับภายนอกหรือแฮชรหัสผ่านซิงโครไนซ์ รหัสผ่านจะถูกเขียนกลับไปยังภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="7ae1b-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="7ae1b-122">ฟังก์ชันการฟังก์ชันนี้ต้องใช้ Azure Premium License (P1 หรือ P2) และขณะนี้ไม่ได้รับการสนับสนุนในพอร์ทัลผู้ดูแลระบบ Office</span><span class="sxs-lookup"><span data-stu-id="7ae1b-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
