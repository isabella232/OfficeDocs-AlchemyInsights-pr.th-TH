---
title: โซลูชันสำหรับปัญหาในการติดตั้ง office บนเซิร์ฟเวอร์เทอร์มินัล
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: df1a50031196fbd79662cee620fc41c7be14e179
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738476"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="1c8a4-102">โซลูชันสำหรับปัญหาในการติดตั้ง office บนเซิร์ฟเวอร์เทอร์มินัล</span><span class="sxs-lookup"><span data-stu-id="1c8a4-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="1c8a4-103">เมื่อต้องการใช้การเปิดใช้งานคอมพิวเตอร์ที่แชร์คุณจะต้องมีการสมัครใช้งานที่มีแอป Microsoft ๓๖๕สำหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="1c8a4-103">To use shared computer activation, you must have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>
  
- <span data-ttu-id="1c8a4-104">ตรวจสอบว่าเปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์แล้ว</span><span class="sxs-lookup"><span data-stu-id="1c8a4-104">Verify that shared computer activation is enabled</span></span>
- <span data-ttu-id="1c8a4-105">ตรวจสอบว่าการเปิดใช้งานเสร็จสมบูรณ์แล้ว</span><span class="sxs-lookup"><span data-stu-id="1c8a4-105">Verify that activation succeeded</span></span>
- <span data-ttu-id="1c8a4-106">ตรวจทานข้อความแสดงข้อผิดพลาดสำหรับการเปิดใช้งานคอมพิวเตอร์ที่แชร์:</span><span class="sxs-lookup"><span data-stu-id="1c8a4-106">Review error messages for shared computer activation:</span></span>
- <span data-ttu-id="1c8a4-107">"ผลิตภัณฑ์ที่เราพบในบัญชีผู้ใช้ของคุณไม่สามารถใช้เพื่อเปิดใช้งาน Office ในสถานการณ์คอมพิวเตอร์ที่แชร์ได้"</span><span class="sxs-lookup"><span data-stu-id="1c8a4-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="1c8a4-108">ข้อผิดพลาดนี้หมายความว่าคุณไม่มีการสมัครใช้งานที่มีแอป Microsoft ๓๖๕สำหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="1c8a4-108">This error means that you don't have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>

<span data-ttu-id="1c8a4-109">"ผลิตภัณฑ์ที่ไม่มีสิทธิ์การทำงาน"</span><span class="sxs-lookup"><span data-stu-id="1c8a4-109">"Unlicensed Product"</span></span>

- <span data-ttu-id="1c8a4-110">ตรวจสอบว่าผู้ใช้ได้รับมอบหมายสิทธิ์การใช้งานสำหรับแอป Microsoft ๓๖๕สำหรับองค์กรหรือไม่</span><span class="sxs-lookup"><span data-stu-id="1c8a4-110">Check that the user is assigned a license for Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="1c8a4-111">ตรวจสอบว่าผู้ใช้ลงชื่อเข้าใช้ด้วยบัญชีผู้ใช้ของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="1c8a4-111">Check that the user signs in with their user account.</span></span>
- <span data-ttu-id="1c8a4-112">ตรวจสอบว่ามีการเชื่อมต่อระหว่างคอมพิวเตอร์ที่ใช้ร่วมกันและอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="1c8a4-112">Check that there is connectivity between the shared computer and the Internet.</span></span>

<span data-ttu-id="1c8a4-113">สำหรับเคล็ดลับในการแก้ไขปัญหาอื่นๆโปรดดู: [แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="1c8a4-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span></span>