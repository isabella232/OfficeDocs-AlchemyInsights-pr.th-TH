---
title: เปิดใช้งานการเขียนย้อนกลับรหัสผ่านในการเชื่อมต่อ AD Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204643"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="6af0f-102">เปิดใช้งานการเขียนย้อนกลับรหัสผ่านในการเชื่อมต่อ AD Azure</span><span class="sxs-lookup"><span data-stu-id="6af0f-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="6af0f-103">เมื่อต้องการเปิดใช้งานการเขียนกลับการตั้งค่ารหัสผ่านด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="6af0f-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="6af0f-104">จากเซิร์ฟเวอร์การเชื่อมต่อ AD Azure ของคุณ ให้ทําตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="6af0f-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="6af0f-105">เข้าสู่ระบบไปยังเซิร์ฟเวอร์การเชื่อมต่อ AD Azure ของคุณและเริ่มตัวช่วยสร้าง**การตั้งค่าคอนฟิกการเชื่อมต่อ AD Azure**</span><span class="sxs-lookup"><span data-stu-id="6af0f-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="6af0f-106">บนหน้า**ยินดีต้อนรับ**ให้คลิก**กําหนดค่า**</span><span class="sxs-lookup"><span data-stu-id="6af0f-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="6af0f-107">บนหน้า**งานเพิ่มเติม**ให้เลือก**กําหนดตัวเลือกการทําข้อมูลให้ตรงกันเอง**แล้วคลิก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="6af0f-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="6af0f-108">บนหน้า**เชื่อมต่อกับ Azure AD**ให้ใส่ข้อมูลประจําตัวของผู้ดูแลระบบส่วนกลางสําหรับผู้เช่า Azure ของคุณ แล้วคลิก ถัดไป</span><span class="sxs-lookup"><span data-stu-id="6af0f-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="6af0f-109">บนหน้า**เชื่อมต่อไดเรกทอรี**และ**การกรองโดเมน/OU**ให้คลิก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="6af0f-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="6af0f-110">บนหน้า**คุณลักษณะตัวเลือก**ให้เลือกกล่องที่อยู่ถัดจาก**การเขียนกลับรหัสผ่าน**แล้วคลิก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="6af0f-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="6af0f-111">บนหน้า**พร้อมที่จะตั้งค่าคอนฟิก**ให้คลิก**กําหนดค่า**และรอให้กระบวนการเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="6af0f-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="6af0f-112">เมื่อคุณเห็นการตั้งค่าคอนฟิกเสร็จสิ้น ให้คลิก**ออก**</span><span class="sxs-lookup"><span data-stu-id="6af0f-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="6af0f-113">ด้วยการเปิดใช้งานการเขียนย้อนกลับรหัสผ่านในการเชื่อมต่อ AD Azure ตอนนี้กําหนดค่า Azure AD SSPR สําหรับเขียนกลับ</span><span class="sxs-lookup"><span data-stu-id="6af0f-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="6af0f-114">เมื่อต้องการเปิดใช้งาน writeback รหัสผ่านใน SSPR ให้ทําตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="6af0f-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="6af0f-115">ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้บัญชีผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="6af0f-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="6af0f-116">ค้นหาและเลือก**ไดเรกทอรีที่ใช้งานอยู่ของ Azure**คลิก**รีเซ็ตรหัสผ่าน**จากนั้นเลือก**การรวมในสถานที่**</span><span class="sxs-lookup"><span data-stu-id="6af0f-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="6af0f-117">ตั้งค่าตัวเลือกสําหรับ**เขียนรหัสผ่านกลับไปยังไดเรกทอรีในสถานของคุณ\*\*\*\*Yes**</span><span class="sxs-lookup"><span data-stu-id="6af0f-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="6af0f-118">ตั้งค่าตัวเลือกสําหรับ**อนุญาตให้ผู้ใช้ปลดล็อกบัญชีโดยไม่ต้องรีเซ็ตรหัสผ่านใหม่\*\*\*\*หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="6af0f-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="6af0f-119">เมื่อพร้อมแล้ว ให้คลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="6af0f-119">When ready, click **Save**.</span></span>

<span data-ttu-id="6af0f-120">สําหรับข้อมูลเพิ่มเติม ให้ดูเปิดใช้งาน Azure Active Directory รีเซ็ต[รหัสผ่านบริการตนเองเพื่อสภาพแวดล้อมในสถานที่](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="6af0f-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
