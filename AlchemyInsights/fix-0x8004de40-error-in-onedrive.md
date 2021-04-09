---
title: แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649767"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4902c-102">แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="4902c-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4902c-103">ถ้าคุณเรียกใช้ Windows 7 และได้รับข้อผิดพลาดนี้ อัปเดตเพื่อเปิดใช้งาน[TLS 1.1 และ TLS 1.2 เป็นโพรโทคอลที่ปลอดภัยเริ่มต้นใน WinHTTP ใน Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span><span class="sxs-lookup"><span data-stu-id="4902c-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="4902c-104">ถ้าคุณใช้งาน Windows 10 และคุณได้รับข้อผิดพลาด0x8004de40 OneDrive:</span><span class="sxs-lookup"><span data-stu-id="4902c-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4902c-105">เริ่มระบบคอมพิวเตอร์ที่ได้รับผลกระทบใหม่ขณะเชื่อมต่อกับโดเมนไดเรกทอรี Acitve ของคุณ</span><span class="sxs-lookup"><span data-stu-id="4902c-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4902c-106">ถ้าการเริ่มต้นระบบใหม่ไม่สามารถแก้ไขปัญหาได้ ให้ยกเลิกการเข้าร่วมและเข้าร่วมอุปกรณ์ของคุณอีกครั้งจาก Azure AD</span><span class="sxs-lookup"><span data-stu-id="4902c-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4902c-107">**หมายเหตุ**: คุณควรอยู่บนเครือข่ายขององค์กรขณะปฏิบัติตามขั้นตอนเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="4902c-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4902c-108">อย่าปฏิบัติตามขั้นตอนเหล่านี้เมื่อคุณไม่ได้เชื่อมต่อกับโครงสร้างพื้นฐานของบริษัทของคุณ (ตัวอย่างเช่น ขณะเดินทาง)</span><span class="sxs-lookup"><span data-stu-id="4902c-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="4902c-109">เปิดพร้อมท์ของสั่งด้วยสิทธิ์ผู้ดูแล **โดย** การเลือก เริ่ม คลิกขวาที่ **พร้อมท์** สั่ง **แล้วเลือก เรียกใช้ในฐานะ** ผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="4902c-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="4902c-110">พิมพ์ *dsregcmd /leave* แล้วกด **Enter**</span><span class="sxs-lookup"><span data-stu-id="4902c-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="4902c-111">เมื่อเสร็จสมบูรณ์ ให้พิมพ์ *dsregcmd /join* แล้วกด **Enter**</span><span class="sxs-lookup"><span data-stu-id="4902c-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="4902c-112">เมื่อเสร็จสมบูรณ์ ให้ปิดพร้อมท์ของสั่ง</span><span class="sxs-lookup"><span data-stu-id="4902c-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="4902c-113">เริ่มระบบคอมพิวเตอร์ใหม่ แล้วเข้าสู่ระบบ OneDrive</span><span class="sxs-lookup"><span data-stu-id="4902c-113">Reboot the computer, and log into OneDrive.</span></span>