---
title: เปิดใช้งานการเขียนกลับรหัสผ่านใน Azure AD Connect
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
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560459"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="f079a-102">เปิดใช้งานการเขียนกลับรหัสผ่านใน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f079a-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="f079a-103">เมื่อต้องการเปิดใช้งานการตั้งค่ารหัสผ่านใหม่แบบบริการตนเองก่อนอื่นให้เปิดใช้งานตัวเลือก writeback ใน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f079a-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="f079a-104">จากเซิร์ฟเวอร์ Azure AD Connect ของคุณให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f079a-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="f079a-105">ลงชื่อเข้าใช้เซิร์ฟเวอร์ Azure AD Connect ของคุณแล้วเริ่มตัวช่วยสร้างการกำหนดค่าการ **เชื่อมต่อ AZURE ad**</span><span class="sxs-lookup"><span data-stu-id="f079a-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="f079a-106">บนหน้า **ยินดีต้อนรับ** ให้คลิก **กำหนดค่า**</span><span class="sxs-lookup"><span data-stu-id="f079a-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="f079a-107">บนหน้า **งานเพิ่มเติม** ให้เลือก **กำหนดตัวเลือกการซิงโครไนซ์** แล้วคลิก **ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="f079a-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="f079a-108">บนหน้าการ **เชื่อมต่อกับ AZURE AD** ให้ใส่ข้อมูลประจำตัวของผู้ดูแลระบบส่วนกลางสำหรับผู้เช่า Azure ของคุณแล้วคลิก **ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="f079a-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="f079a-109">บนหน้า **เชื่อมต่อไดเรกทอรี** และ **โดเมน/OU** การกรองคลิก **ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="f079a-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="f079a-110">บนหน้า **ฟีเจอร์เพิ่มเติม** ให้เลือกกล่องที่อยู่ถัดจาก **writeback รหัสผ่าน** แล้วคลิก **ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="f079a-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="f079a-111">บนหน้า **พร้อมที่จะกำหนดค่า** ให้คลิก **กำหนดค่า** แล้วรอให้กระบวนการเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="f079a-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="f079a-112">เมื่อคุณเห็นการกำหนดค่าเสร็จสิ้นให้คลิก **ออก**</span><span class="sxs-lookup"><span data-stu-id="f079a-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="f079a-113">ด้วยการเปิดใช้งานการเขียนกลับของรหัสผ่านใน Azure AD ให้กำหนดค่า Azure AD SSPR สำหรับ writeback</span><span class="sxs-lookup"><span data-stu-id="f079a-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="f079a-114">เมื่อต้องการเปิดใช้งานการเขียนกลับรหัสผ่านใน SSPR ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f079a-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="f079a-115">ลงชื่อเข้าใช้พอร์ทัล Azure โดยใช้บัญชีผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="f079a-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="f079a-116">ค้นหาและเลือก **Azure Active directory** ให้คลิกการ **ตั้งค่ารหัสผ่านใหม่** แล้วคลิกการ **รวมภายในองค์กร**</span><span class="sxs-lookup"><span data-stu-id="f079a-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="f079a-117">ตั้งค่าตัวเลือกสำหรับการ **เขียนรหัสผ่านใหม่ไปยังไดเรกทอรีภายในองค์กรของคุณใช่หรือไม่** **Yes**</span><span class="sxs-lookup"><span data-stu-id="f079a-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="f079a-118">ตั้งค่าตัวเลือกสำหรับ **อนุญาตให้ผู้ใช้สามารถปลดล็อกบัญชีได้โดยไม่ต้องรีเซ็ตรหัสผ่านของพวกเขาใช่หรือไม่** **Yes**</span><span class="sxs-lookup"><span data-stu-id="f079a-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="f079a-119">เมื่อพร้อมแล้วให้คลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="f079a-119">When ready, click **Save**.</span></span>

<span data-ttu-id="f079a-120">สำหรับข้อมูลเพิ่มเติมให้ดูที่[เปิดใช้งาน Azure Active directory ตั้งค่ารหัสผ่านใหม่แบบบริการตนเองในสภาพแวดล้อมภายในองค์กร](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="f079a-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="f079a-121">เมื่อผู้ดูแลระบบตั้งค่ารหัสผ่านของผู้ใช้ใหม่ในพอร์ทัล Azure ถ้าผู้ใช้นั้นเป็นผู้ติดต่อกับภายนอกหรือการซิงโครไนซ์แฮชของรหัสผ่านแล้วรหัสผ่านจะถูกเขียนกลับไปยังภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="f079a-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="f079a-122">ฟังก์ชันการทำงานนี้ไม่ได้รับการสนับสนุนในพอร์ทัลการดูแลระบบ Office ในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="f079a-122">This functionality is currently not supported in the Office Admin portal.</span></span>