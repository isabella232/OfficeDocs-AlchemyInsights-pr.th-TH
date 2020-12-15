---
title: ใช้ Microsoft Intune ในการจัดการการเข้าถึงเว็บใน Microsoft Edge สำหรับ iOS และ Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679610"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="b6089-102">ใช้ Microsoft Intune ในการจัดการการเข้าถึงเว็บใน Microsoft Edge สำหรับ iOS และ Android</span><span class="sxs-lookup"><span data-stu-id="b6089-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="b6089-103">Microsoft Edge for iOS และ Android ช่วยให้ผู้ใช้สามารถเรียกดูเว็บจากหลายโปรไฟล์ที่แยกจากกันได้อย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="b6089-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="b6089-104">ความสามารถในการป้องกันที่ดีที่สุดสำหรับข้อมูล Microsoft ๓๖๕จะพร้อมใช้งานเมื่อคุณสมัครใช้งาน office Mobility + ชุดการรักษาความปลอดภัยซึ่งรวมถึง Microsoft Intune และ Azure Active Directory Premium เช่นการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="b6089-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="b6089-105">อย่างน้อยที่สุดคุณจะต้องปรับใช้นโยบายการเข้าถึงตามเงื่อนไขที่ (1) ช่วยให้ผู้ใช้เชื่อมต่อจากอุปกรณ์เคลื่อนที่ไปยัง Microsoft Edge สำหรับ iOS และ Android และ (2) ใช้นโยบายการป้องกันแอป Microsoft Intune ที่มีประสบการณ์การใช้งานการป้องกันที่ได้รับการป้องกัน</span><span class="sxs-lookup"><span data-stu-id="b6089-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="b6089-106">เมื่อต้องการทำความเข้าใจวิธีที่คุณสามารถใช้การเข้าถึงแบบมีเงื่อนไขและนโยบายให้ดู:</span><span class="sxs-lookup"><span data-stu-id="b6089-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="b6089-107">นำนโยบายการเข้าถึงแบบมีเงื่อนไขของ Azure Active Directory ไปใช้</span><span class="sxs-lookup"><span data-stu-id="b6089-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="b6089-108">สร้างนโยบายการป้องกันแอป Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b6089-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="b6089-109">ใช้การลงชื่อเข้าใช้ครั้งเดียวสำหรับ Azure Active Directory –แอปเว็บที่เชื่อมต่ออยู่ในเบราว์เซอร์ที่มีการป้องกันด้วยนโยบาย</span><span class="sxs-lookup"><span data-stu-id="b6089-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="b6089-110">ใช้การกำหนดค่าแอปเพื่อจัดการประสบการณ์การใช้งานการเรียกดู</span><span class="sxs-lookup"><span data-stu-id="b6089-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="b6089-111">อนุญาตให้ใช้บัญชีที่ทำงานและที่โรงเรียนเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="b6089-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="b6089-112">ปรับใช้นโยบายการกำหนดค่าทั่วไปของแอป</span><span class="sxs-lookup"><span data-stu-id="b6089-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="b6089-113">การปรับใช้นโยบายการกำหนดค่าแอปสำหรับการป้องกันข้อมูล</span><span class="sxs-lookup"><span data-stu-id="b6089-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="b6089-114">ใช้ตัวจัดการจุดสิ้นสุดของ Microsoft เพื่อปรับใช้นโยบายการกำหนดค่าแอป</span><span class="sxs-lookup"><span data-stu-id="b6089-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="b6089-115">เมื่อต้องการเรียนรู้วิธีการเข้าถึงบันทึกของแอปที่ได้รับการจัดการให้ดู[ที่ใช้ Microsoft Edge สำหรับ iOS และ Android เพื่อเข้าถึงบันทึกของแอปที่มีการจัดการ](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="b6089-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
