---
title: เปิดใช้งาน Writeback รหัสผ่านใน Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093374"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="fe4c9-102">เปิดใช้งาน Writeback รหัสผ่านใน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="fe4c9-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="fe4c9-103">เมื่อต้องการเปิดใช้งาน Writeback รีเซ็ตรหัสผ่านแบบบริการตนเอง ก่อนอื่น ให้เปิดใช้งานตัวเลือก Writeback ใน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="fe4c9-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="fe4c9-104">จากเซิร์ฟเวอร์ Azure AD Connect ของคุณ ให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="fe4c9-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="fe4c9-105">ลงชื่อเข้าใช้เซิร์ฟเวอร์ Azure AD Connect ของคุณและเริ่มตัวช่วยสร้างการ **กําหนดค่า Azure AD Connect**</span><span class="sxs-lookup"><span data-stu-id="fe4c9-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="fe4c9-106">บนหน้า **ยินดีต้อนรับ** ให้คลิก **กําหนด** ค่า</span><span class="sxs-lookup"><span data-stu-id="fe4c9-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="fe4c9-107">บนหน้า **งานเพิ่มเติม** ให้เลือกตัวเลือก **ปรับแต่งการ** ซิงโครไนซ์ **แล้วคลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="fe4c9-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="fe4c9-108">บนหน้า **เชื่อมต่อไปยัง Azure AD ให้** ใส่ข้อมูลรับรองความถูกต้องของผู้ดูแลระบบส่วนกลางของผู้เช่า Azure ของคุณ **แล้วคลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="fe4c9-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="fe4c9-109">บนหน้า **การกรอง เชื่อมต่อ** ไดเรกทอรี **และโดเมน/OU** **ให้คลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="fe4c9-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="fe4c9-110">บนหน้า **ฟีเจอร์เพิ่มเติม** ให้เลือกกล่องที่อยู่ถัดจาก Password **Writeback\*\*\*\*แล้วคลิก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="fe4c9-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="fe4c9-111">บนหน้า **พร้อมที่จะกําหนดค่า** ให้คลิก **กําหนด** ค่า และรอให้กระบวนการเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="fe4c9-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="fe4c9-112">เมื่อคุณเห็นการกําหนดค่าเสร็จสิ้น **ให้คลิก** ออก</span><span class="sxs-lookup"><span data-stu-id="fe4c9-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="fe4c9-113">เมื่อเปิดใช้งาน Writeback ของรหัสผ่านใน Azure AD Connect ให้กําหนดค่า Azure AD SSPR for writeback</span><span class="sxs-lookup"><span data-stu-id="fe4c9-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="fe4c9-114">เมื่อต้องการเปิดใช้งาน Writeback ของรหัสผ่านใน SSPR ให้เสร็จสิ้นขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="fe4c9-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="fe4c9-115">ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้บัญชีผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="fe4c9-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="fe4c9-116">ค้นหาและเลือก **Azure Active Directory\*\*\*\*คลิกรีเซ็ต** รหัสผ่าน จากนั้นคลิก **การรวมภายใน** องค์กร</span><span class="sxs-lookup"><span data-stu-id="fe4c9-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="fe4c9-117">ตั้งค่าตัวเลือกให้ **เขียนรหัสผ่านกลับลงในไดเรกทอรีภายในองค์กรของคุณใช่ไหม\*\*\*\*เป็น** ใช่</span><span class="sxs-lookup"><span data-stu-id="fe4c9-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="fe4c9-118">ตั้งค่าตัวเลือกให้ **อนุญาตให้ผู้ใช้ปลดล็อกบัญชีโดยไม่ต้องรีเซ็ตรหัสผ่านของพวกเขาหรือไม่\*\*\*\*เป็น** ใช่</span><span class="sxs-lookup"><span data-stu-id="fe4c9-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="fe4c9-119">เมื่อพร้อม **ให้คลิก** บันทึก</span><span class="sxs-lookup"><span data-stu-id="fe4c9-119">When ready, click **Save**.</span></span>

<span data-ttu-id="fe4c9-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="fe4c9-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="fe4c9-121">เมื่อผู้ดูแลระบบรีเซ็ตรหัสผ่านของผู้ใช้ในพอร์ทัล Azure ถ้าผู้ใช้นั้นติดต่อกับภายนอกหรือแฮชรหัสผ่านซิงโครไนซ์ รหัสผ่านจะถูกเขียนกลับไปยังภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="fe4c9-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="fe4c9-122">หน้าที่การใช้งานนี้ต้องใช้ Azure Premium License (P1 หรือ P2) และในขณะนี้ไม่ได้รับการสนับสนุนในพอร์ทัลผู้ดูแลระบบ Office</span><span class="sxs-lookup"><span data-stu-id="fe4c9-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
