---
title: วิธีแก้ไขปัญหาสำหรับปัญหาที่ล้อมรอบการติดตั้ง office บนเทอร์มินัลเซิร์ฟเวอร์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: bed91bf59219a19d5742d3ca4a61718c34b5c774
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501494"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="db596-102">วิธีแก้ไขปัญหาสำหรับปัญหาที่ล้อมรอบการติดตั้ง office บนเทอร์มินัลเซิร์ฟเวอร์</span><span class="sxs-lookup"><span data-stu-id="db596-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="db596-103">เมื่อต้องการใช้เปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน คุณต้องมีแผนการ Office 365 ที่มี Office 365 ProPlus</span><span class="sxs-lookup"><span data-stu-id="db596-103">To use shared computer activation, you must have an Office 365 plan that includes Office 365 ProPlus.</span></span>
  
- <span data-ttu-id="db596-104">ตรวจสอบว่า เปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันถูกเปิดใช้งาน Office 365 ProPlus</span><span class="sxs-lookup"><span data-stu-id="db596-104">Verify that shared computer activation is enabled for Office 365 ProPlus</span></span>
    
- <span data-ttu-id="db596-105">ตรวจสอบว่า มีการเปิดใช้งานสำหรับ Office 365 ProPlus ได้สำเร็จ</span><span class="sxs-lookup"><span data-stu-id="db596-105">Verify that activation for Office 365 ProPlus succeeded</span></span>
    
- <span data-ttu-id="db596-106">ตรวจทานข้อความแสดงข้อผิดพลาดสำหรับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน:</span><span class="sxs-lookup"><span data-stu-id="db596-106">Review error messages for shared computer activation:</span></span>
    
  - <span data-ttu-id="db596-107">"ผลิตภัณฑ์เราพบในบัญชีของคุณไม่สามารถใช้เพื่อเปิดใช้งาน Office ในสถานการณ์จำลองในคอมพิวเตอร์ที่ใช้ร่วมกัน"</span><span class="sxs-lookup"><span data-stu-id="db596-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="db596-108">ข้อผิดพลาดนี้หมายความ ว่า คุณไม่มีแผนการ Office 365 ที่มี Office 365 ProPlus</span><span class="sxs-lookup"><span data-stu-id="db596-108">This error means that you don't have an Office 365 plan that includes Office 365 ProPlus.</span></span>
    
  - <span data-ttu-id="db596-109">"ผลิตภัณฑ์สิทธิ์"</span><span class="sxs-lookup"><span data-stu-id="db596-109">"Unlicensed Product"</span></span>
    
  - <span data-ttu-id="db596-110">ตรวจสอบว่า ผู้ใช้มีกำหนดสิทธิ์การใช้งานสำหรับ Office 365 ProPlus</span><span class="sxs-lookup"><span data-stu-id="db596-110">Check that the user is assigned a license for Office 365 ProPlus.</span></span>
    
  - <span data-ttu-id="db596-111">ตรวจสอบว่า ผู้ใช้ที่ลงทะเบียน ด้วยบัญชีผู้ใช้ของตนเองสำหรับ Office 365</span><span class="sxs-lookup"><span data-stu-id="db596-111">Check that the user signs in with her user account for Office 365</span></span>
    
  - <span data-ttu-id="db596-112">ตรวจสอบว่า มีการเชื่อมต่อระหว่างคอมพิวเตอร์ที่ใช้ร่วมกันและอินเทอร์เน็ตหรือไม่</span><span class="sxs-lookup"><span data-stu-id="db596-112">Check that there is connectivity between the shared computer and the Internet.</span></span>
    
<span data-ttu-id="db596-113">สำหรับเคล็ดลับการแก้ไขปัญหาอื่น ๆ โปรดดูที่:[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสำหรับ Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="db596-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span></span>
  

