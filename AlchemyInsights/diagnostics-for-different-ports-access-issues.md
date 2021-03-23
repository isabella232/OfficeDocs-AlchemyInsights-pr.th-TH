---
title: การวินิจฉัยปัญหาการเข้าถึงพอร์ตต่างๆ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036806"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="9be36-102">การวินิจฉัยปัญหาการเข้าถึงพอร์ตต่างๆ</span><span class="sxs-lookup"><span data-stu-id="9be36-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="9be36-103">เมื่อต้องการแก้ไขปัญหาการเข้าถึงพอร์ตต่างๆ ให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9be36-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="9be36-104">หยุด/จัดการเครื่องเสมือน (VM) จากพอร์ทัล เริ่ม VM ใหม่ และทดสอบอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="9be36-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="9be36-105">ตรวจสอบการตั้งค่าเครือข่ายของ VM ของคุณเพื่อตรวจสอบว่าคุณมีการรับส่งข้อมูลบล็อกกลุ่มความปลอดภัยของเครือข่าย (NSG) หรือไม่</span><span class="sxs-lookup"><span data-stu-id="9be36-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="9be36-106">คุณยังสามารถใช้เครื่องมือตรวจสอบ [IP ของ Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) เพื่อตรวจสอบ NSGs ที่บล็อกการรับส่งข้อมูล, เส้นทาง User-Defined (UUDR) สร้างเส้นทางการรับส่งข้อมูลของคุณใหม่ไปยังภายในองค์กร ('Default Route' 0.0.0.0/0) หรือกับผู้ตรวจสอบเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="9be36-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="9be36-107">ถ้าคุณยังคงพบปัญหาหลังจากลองปฏิบัติตามขั้นตอนด้านบน โปรดระบุชื่อ VM และพอร์ต TCP ที่คุณพยายามส่งจดหมายเพื่อแก้ปัญหาเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="9be36-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="9be36-108">**เอกสารที่แนะนา**</span><span class="sxs-lookup"><span data-stu-id="9be36-108">**Recommended Documents**</span></span>

[<span data-ttu-id="9be36-109">ข้อจํากัดและข้อเสนอแนะในการส่งอีเมลขาออกผ่านพอร์ต 25</span><span class="sxs-lookup"><span data-stu-id="9be36-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)