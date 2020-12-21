---
title: จัดการกลุ่มแอปโดยใช้พอร์ทัล Azure สำหรับเดสก์ท็อปเสมือนของ Windows
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
- "9003956"
- "7013"
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722053"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a><span data-ttu-id="3ed0c-102">จัดการกลุ่มแอปโดยใช้พอร์ทัล Azure สำหรับเดสก์ท็อปเสมือนของ Windows</span><span class="sxs-lookup"><span data-stu-id="3ed0c-102">Manage app groups by using the Azure portal for Windows Virtual Desktop</span></span>

<span data-ttu-id="3ed0c-103">กลุ่มแอปเริ่มต้นที่สร้างขึ้นสำหรับพูลโปรแกรมโฮสต์เดสก์ท็อปเสมือนใหม่ของ Windows จะเผยแพร่เดสก์ท็อปแบบเต็ม</span><span class="sxs-lookup"><span data-stu-id="3ed0c-103">The default app group created for a new Windows Virtual Desktop host pool also publishes the full desktop.</span></span> <span data-ttu-id="3ed0c-104">นอกจากนี้การใช้พอร์ทัล Azure จะช่วยให้คุณสามารถสร้างกลุ่มแอป RemoteApp อย่างน้อยหนึ่งกลุ่มสำหรับพูลโปรแกรมโฮสต์</span><span class="sxs-lookup"><span data-stu-id="3ed0c-104">In addition, using the Azure portal lets you create one or more RemoteApp app groups for the host pool.</span></span>

<span data-ttu-id="3ed0c-105">กระบวนการปรับใช้จะดำเนินการดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="3ed0c-105">The deployment process will do the following:</span></span>

1. <span data-ttu-id="3ed0c-106">สร้างกลุ่มแอป RemoteApp</span><span class="sxs-lookup"><span data-stu-id="3ed0c-106">Create the RemoteApp app group.</span></span>
2. <span data-ttu-id="3ed0c-107">เพิ่มแอปที่เลือกของคุณลงในกลุ่มแอป</span><span class="sxs-lookup"><span data-stu-id="3ed0c-107">Add your selected apps to the app group.</span></span>
3. <span data-ttu-id="3ed0c-108">ประกาศผู้ใช้แต่ละรายหรือกลุ่มผู้ใช้ไปยังกลุ่มแอป</span><span class="sxs-lookup"><span data-stu-id="3ed0c-108">Publish individual users or user groups to the app group.</span></span>
4. <span data-ttu-id="3ed0c-109">ลงทะเบียนกลุ่มแอปถ้าคุณเลือกที่จะทำเช่นนั้น</span><span class="sxs-lookup"><span data-stu-id="3ed0c-109">Register the app group, if you choose to do so.</span></span>
5. <span data-ttu-id="3ed0c-110">สร้างลิงก์ไปยังแม่แบบตัวจัดการทรัพยากร Azure ตามการกำหนดค่าของคุณซึ่งคุณสามารถดาวน์โหลดและบันทึกได้</span><span class="sxs-lookup"><span data-stu-id="3ed0c-110">Create a link to an Azure Resource Manager template according to your configuration, which you can download and save.</span></span>

<span data-ttu-id="3ed0c-111">เมื่อต้องการสร้างกลุ่ม RemoteApp สำหรับเดสก์ท็อปเสมือนของ Windows ให้ทำตามคำแนะนำใน[จัดการกลุ่มแอปได้ด้วยพอร์ทัล Azure](https://go.microsoft.com/fwlink/?linkid=2129550)</span><span class="sxs-lookup"><span data-stu-id="3ed0c-111">To create a RemoteApp group for Windows Virtual Desktop, follow the instructions in [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span></span>
