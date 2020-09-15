---
title: รหัสข้อผิดพลาด0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office ๒๐๑๓บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้ลองเปิดใช้งานการ ADAL โดยการแก้ไขรีจิสทรี
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709206"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="f8ab9-103">เกิดข้อผิดพลาดขณะเปิดใช้งาน Office ๒๐๑๓บนบริการเดสก์ท็อประยะไกล</span><span class="sxs-lookup"><span data-stu-id="f8ab9-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="f8ab9-104">ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office ๒๐๑๓บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้ลองเปิดใช้งานการ ADAL โดยการแก้ไขรีจิสทรี</span><span class="sxs-lookup"><span data-stu-id="f8ab9-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="f8ab9-105">**รีจิสทรีคีย์**</span><span class="sxs-lookup"><span data-stu-id="f8ab9-105">**Registry key**</span></span>|<span data-ttu-id="f8ab9-106">**ชนิด**</span><span class="sxs-lookup"><span data-stu-id="f8ab9-106">**Type**</span></span>|<span data-ttu-id="f8ab9-107">**ค่า**</span><span class="sxs-lookup"><span data-stu-id="f8ab9-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f8ab9-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="f8ab9-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="f8ab9-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="f8ab9-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="f8ab9-110">1</span><span class="sxs-lookup"><span data-stu-id="f8ab9-110">1</span></span>  <br/> |

<span data-ttu-id="f8ab9-111">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่เปิดใช้งานการรับรองความถูกต้องที่ทันสมัยสำหรับ Office ๒๐๑๓บนอุปกรณ์ Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)</span><span class="sxs-lookup"><span data-stu-id="f8ab9-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="f8ab9-112">ADAL จะถูกเปิดใช้งานตามค่าเริ่มต้นในแอป Microsoft ๓๖๕สำหรับองค์กรและ Office ๒๐๑๖</span><span class="sxs-lookup"><span data-stu-id="f8ab9-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="f8ab9-113">บริการเดสก์ท็อประยะไกล (RDS) ถูกชื่อว่าบริการเทอร์มินัลก่อนหน้านี้</span><span class="sxs-lookup"><span data-stu-id="f8ab9-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  