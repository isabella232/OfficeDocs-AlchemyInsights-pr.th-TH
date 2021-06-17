---
title: ใช้ Microsoft Intuned เพื่อจัดการการเข้าถึงเว็บใน Microsoft Edge for iOS และ Android
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
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989724"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="ae6d3-102">ใช้ Microsoft Intuned เพื่อจัดการการเข้าถึงเว็บใน Microsoft Edge for iOS และ Android</span><span class="sxs-lookup"><span data-stu-id="ae6d3-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="ae6d3-103">Microsoft Edge for iOS และ Android ช่วยให้ผู้ใช้สามารถเรียกดูเว็บจากหลายโปรไฟล์แยกกันโดยสิ้นเชิง</span><span class="sxs-lookup"><span data-stu-id="ae6d3-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="ae6d3-104">ความสามารถในการป้องกันที่กว้างที่สุดของข้อมูล Microsoft 365 จะพร้อมใช้งานเมื่อคุณสมัครใช้งานชุดโปรแกรม Enterprise Mobility + Security ซึ่งรวมถึง Microsoft Intunes และฟีเจอร์ Azure Active Directory Premium เช่น การเข้าถึงตามเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="ae6d3-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="ae6d3-105">อย่างน้อยที่สุด คุณจะต้องการปรับใช้นโยบายการเข้าถึงตามเงื่อนไขที่ (1) ช่วยให้ผู้ใช้เชื่อมต่อจากอุปกรณ์เคลื่อนที่ไปยัง Microsoft Edge for iOS และ Android และนโยบายดังกล่าว (2) ใช้นโยบายการป้องกันแอปของ Microsoft Intuned ที่ให้ประสบการณ์การเรียกดูที่ได้รับการป้องกัน</span><span class="sxs-lookup"><span data-stu-id="ae6d3-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="ae6d3-106">เมื่อต้องการเข้าใจว่าคุณสามารถใช้การเข้าถึงและนโยบายตามเงื่อนไขอย่างไร ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="ae6d3-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="ae6d3-107">ปรับใช้นโยบายการเข้าถึงตามเงื่อนไขของ Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="ae6d3-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="ae6d3-108">สร้างนโยบายการป้องกันแอป Microsoft Intun1</span><span class="sxs-lookup"><span data-stu-id="ae6d3-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="ae6d3-109">ใช้การลงชื่อเข้าระบบครั้งเดียวในแอป Azure Active Directory บนเว็บที่เชื่อมต่อในเบราว์เซอร์ที่มีการป้องกันนโยบาย</span><span class="sxs-lookup"><span data-stu-id="ae6d3-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="ae6d3-110">ใช้การกําหนดค่าแอปเพื่อจัดการประสบการณ์การเรียกดู</span><span class="sxs-lookup"><span data-stu-id="ae6d3-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="ae6d3-111">อนุญาตให้ใช้เฉพาะบัญชีที่โรงเรียนและที่โรงเรียน</span><span class="sxs-lookup"><span data-stu-id="ae6d3-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="ae6d3-112">ปรับใช้นโยบายการกําหนดค่าแอปทั่วไป</span><span class="sxs-lookup"><span data-stu-id="ae6d3-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="ae6d3-113">ปรับใช้นโยบายการกําหนดค่าแอปเพื่อการป้องกันข้อมูล</span><span class="sxs-lookup"><span data-stu-id="ae6d3-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="ae6d3-114">ใช้ตัวจัดการจุดสิ้นสุดของ Microsoft เพื่อปรับใช้นโยบายการกําหนดค่าแอป</span><span class="sxs-lookup"><span data-stu-id="ae6d3-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="ae6d3-115">เมื่อต้องการเรียนรู้วิธีการเข้าถึงบันทึกแอปที่มีการจัดการ ให้ดู [ใช้ Microsoft Edge for iOS และ Android เพื่อเข้าถึงบันทึกแอปที่มี](https://go.microsoft.com/fwlink/?linkid=2132578)การจัดการ</span><span class="sxs-lookup"><span data-stu-id="ae6d3-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
