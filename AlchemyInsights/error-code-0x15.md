---
title: รหัสข้อผิดพลาด 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้ลองเปิดใช้งาน ADAL ด้วยการแก้ไขรีจิสทรี
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703157"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="24d84-103">ข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนบริการเดสก์ท็อประยะไกล</span><span class="sxs-lookup"><span data-stu-id="24d84-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="24d84-104">ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้ลองเปิดใช้งาน ADAL ด้วยการแก้ไขรีจิสทรี</span><span class="sxs-lookup"><span data-stu-id="24d84-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="24d84-105">**คีย์รีจิสทรี**</span><span class="sxs-lookup"><span data-stu-id="24d84-105">**Registry key**</span></span>|<span data-ttu-id="24d84-106">**ชนิด**</span><span class="sxs-lookup"><span data-stu-id="24d84-106">**Type**</span></span>|<span data-ttu-id="24d84-107">**ค่า**</span><span class="sxs-lookup"><span data-stu-id="24d84-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="24d84-108">HKEY_CURRENT_USER\ซอฟต์แวร์\Microsoft\Office\15.0\ทั่วไป\ข้อมูลประจําตัว\เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="24d84-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="24d84-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="24d84-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="24d84-110">1</span><span class="sxs-lookup"><span data-stu-id="24d84-110">1</span></span>  <br/> |

<span data-ttu-id="24d84-111">สําหรับข้อมูลเพิ่มเติม ให้ดู[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สําหรับ Office 2013 บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)</span><span class="sxs-lookup"><span data-stu-id="24d84-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="24d84-112">เปิดใช้งานโดยค่าเริ่มต้นในโปรแกรมประยุกต์ของ Microsoft 365 สําหรับองค์กรและ Office 2016</span><span class="sxs-lookup"><span data-stu-id="24d84-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="24d84-113">บริการเดสก์ท็อประยะไกล (RDS) ได้ก่อนหน้านี้ชื่อบริการเทอร์มินัล</span><span class="sxs-lookup"><span data-stu-id="24d84-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  