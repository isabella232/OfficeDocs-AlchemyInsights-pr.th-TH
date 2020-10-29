---
title: ไฟล์ตามความต้องการ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791313"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="d9524-102">กำหนดค่าไฟล์ตามความต้องการ</span><span class="sxs-lookup"><span data-stu-id="d9524-102">Configure Files On-Demand</span></span>

<span data-ttu-id="d9524-103">ไฟล์ OneDrive ตามความต้องการต้องการการ [อัปเดต windows 10](https://go.microsoft.com/fwlink/p/?linkid=859040) (เวอร์ชัน๑๗๐๙หรือใหม่กว่า) หรือ windows Server ๒๐๑๙และ OneDrive รุ่น17.3.7064.1005 หรือเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="d9524-103">OneDrive Files On-Demand requires [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (version 1709 or later) or Windows Server 2019 and OneDrive build 17.3.7064.1005 or later.</span></span>

<span data-ttu-id="d9524-104">ไฟล์ OneDrive ตามความต้องการของคุณจะช่วยให้คุณสามารถเข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive ได้โดยไม่ต้องดาวน์โหลดทั้งหมดและใช้พื้นที่เก็บข้อมูลบนอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="d9524-104">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="d9524-105">เมื่อต้องการกำหนดค่าไฟล์ตามความต้องการบนพีซีของคุณ:</span><span class="sxs-lookup"><span data-stu-id="d9524-105">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="d9524-106">เลือกไอคอนรูปเมฆสีขาวหรือสีน้ำเงินของ **OneDrive** ในพื้นที่แจ้งให้ทราบของแถบงาน Windows</span><span class="sxs-lookup"><span data-stu-id="d9524-106">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="d9524-107">เลือก **วิธีใช้ &** ไอคอนเกียร์การตั้งค่า > **การตั้งค่า**</span><span class="sxs-lookup"><span data-stu-id="d9524-107">Select the **Help & Settings** gear icon > **Settings** .</span></span>
2. <span data-ttu-id="d9524-108">บนแท็บ **การตั้งค่า** ให้เลือก **บันทึกช่องว่างและดาวน์โหลดไฟล์ขณะที่คุณใช้กล่องเหล่านั้น**</span><span class="sxs-lookup"><span data-stu-id="d9524-108">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="d9524-109">นอกจากนี้คุณยังสามารถกำหนดค่าไฟล์ตามความต้องการโดยใช้รีจิสทรีได้อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="d9524-109">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="d9524-110">ถ้าคุณปิดใช้งานการตั้งค่านี้ผู้ใช้ Windows 10 จะมีลักษณะการทำงานการซิงค์เดียวกันกับผู้ใช้ Windows เวอร์ชันก่อนหน้าและไม่สามารถเปิดไฟล์ตามความต้องการได้</span><span class="sxs-lookup"><span data-stu-id="d9524-110">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="d9524-111">ถ้าคุณไม่ได้กำหนดค่าการตั้งค่านี้ผู้ใช้สามารถเปิดหรือปิดไฟล์ตามความต้องการได้</span><span class="sxs-lookup"><span data-stu-id="d9524-111">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="d9524-112">การเปิดใช้งานนโยบายนี้จะตั้งค่าคีย์รีจิสทรีต่อไปนี้เป็น1</span><span class="sxs-lookup"><span data-stu-id="d9524-112">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="d9524-113">การปิดใช้งานนโยบายนี้จะตั้งค่าคีย์รีจิสทรีต่อไปนี้เป็น0</span><span class="sxs-lookup"><span data-stu-id="d9524-113">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="d9524-114">ถ้าคุณไม่เห็นตัวเลือกไฟล์ตามความต้องการใน "การตั้งค่า" ให้ตรวจสอบให้แน่ใจว่าชนิดเริ่มต้นของบริการ "Windows Cloud Files Filter Driver" ถูกตั้งค่าเป็น 2 (AUTO_START)</span><span class="sxs-lookup"><span data-stu-id="d9524-114">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="d9524-115">การเปิดใช้งานฟีเจอร์นี้จะตั้งค่าคีย์รีจิสทรีต่อไปนี้เป็น2</span><span class="sxs-lookup"><span data-stu-id="d9524-115">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`