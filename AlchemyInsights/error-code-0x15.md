---
title: รหัสข้อผิดพลาด 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการกำหนดใช้บริการเดสก์ท็อประยะไกล (RDS) พิจารณาการเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499401"
---
<span data-ttu-id="1e8a4-103">ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการกำหนดใช้บริการเดสก์ท็อประยะไกล (RDS) พิจารณาการเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี</span><span class="sxs-lookup"><span data-stu-id="1e8a4-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="1e8a4-104">**คีย์รีจิสทรี**</span><span class="sxs-lookup"><span data-stu-id="1e8a4-104">**Registry key**</span></span>|<span data-ttu-id="1e8a4-105">พิมพ์</span><span class="sxs-lookup"><span data-stu-id="1e8a4-105">**Type**</span></span>|<span data-ttu-id="1e8a4-106">ค่า</span><span class="sxs-lookup"><span data-stu-id="1e8a4-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1e8a4-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="1e8a4-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="1e8a4-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="1e8a4-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="1e8a4-109">1</span><span class="sxs-lookup"><span data-stu-id="1e8a4-109">1</span></span>  <br/> |
   
<span data-ttu-id="1e8a4-110">สำหรับข้อมูลเพิ่มเติม ให้ดู[เปิดใช้งานการพิสูจน์ตัวจริงแบบสมัยใหม่สำหรับ 2013 Office บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)</span><span class="sxs-lookup"><span data-stu-id="1e8a4-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="1e8a4-p101">ADAL ถูกเปิดใช้งาน โดยค่าเริ่มต้นใน Office 365 ProPlus และ Office 2016 บริการเดสก์ท็อประยะไกล (RDS) > ก่อนหน้านี้เคยใช้ชื่อบริการเทอร์มินัล</span><span class="sxs-lookup"><span data-stu-id="1e8a4-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

