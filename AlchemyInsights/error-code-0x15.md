---
title: รหัสข้อผิดพลาด 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการกำหนดใช้บริการเดสก์ท็อประยะไกล (RDS) พิจารณาการเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402758"
---
<span data-ttu-id="a97dd-103">ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการกำหนดใช้บริการเดสก์ท็อประยะไกล (RDS) พิจารณาการเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี</span><span class="sxs-lookup"><span data-stu-id="a97dd-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="a97dd-104">**คีย์รีจิสทรี**</span><span class="sxs-lookup"><span data-stu-id="a97dd-104">**Registry key**</span></span>|<span data-ttu-id="a97dd-105">**ชนิด**</span><span class="sxs-lookup"><span data-stu-id="a97dd-105">**Type**</span></span>|<span data-ttu-id="a97dd-106">**ค่า**</span><span class="sxs-lookup"><span data-stu-id="a97dd-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a97dd-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="a97dd-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="a97dd-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="a97dd-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="a97dd-109">1</span><span class="sxs-lookup"><span data-stu-id="a97dd-109">1</span></span>  <br/> |
   
<span data-ttu-id="a97dd-110">สำหรับข้อมูลเพิ่มเติม ให้ดู[เปิดใช้งานการพิสูจน์ตัวจริงแบบสมัยใหม่สำหรับ 2013 Office บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)</span><span class="sxs-lookup"><span data-stu-id="a97dd-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="a97dd-111">ADAL ถูกเปิดใช้งาน โดยค่าเริ่มต้นใน Office 365 ProPlus และ Office 2016</span><span class="sxs-lookup"><span data-stu-id="a97dd-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="a97dd-112">บริการเดสก์ท็อประยะไกล (RDS) > ก่อนหน้านี้เคยใช้ชื่อบริการเทอร์มินัล</span><span class="sxs-lookup"><span data-stu-id="a97dd-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

