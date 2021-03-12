---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709125"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="7aaf9-102">การแก้ไขแอป Microsoft 365 ข้อความ "แพลตฟอร์มที่เชื่อถือได้ของคอมพิวเตอร์ของคุณไม่ฟังก์ชันอย่างถูกต้อง"</span><span class="sxs-lookup"><span data-stu-id="7aaf9-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="7aaf9-103">เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ลองต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7aaf9-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="7aaf9-104">ติดตั้งการอัปเดตล่าสุดของ[Windows](https://support.microsoft.com/help/4027667/windows-10-update) [และ Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="7aaf9-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7aaf9-105">[ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="7aaf9-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7aaf9-106">**หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว</span><span class="sxs-lookup"><span data-stu-id="7aaf9-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7aaf9-107">(เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7aaf9-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7aaf9-108">ลองกระบวนการ [กู้คืนผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) เพื่อแก้ไขความล้มเหลวของ Trusted Platform Module (TPM)</span><span class="sxs-lookup"><span data-stu-id="7aaf9-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="7aaf9-109">ตั้งค่า EnableADAL = 0 โดยใช้ขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7aaf9-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="7aaf9-110">คลิกขวาที่ปุ่ม เริ่ม ของ Windows เลือก **เรียกใช้** พิมพ์ **regedit\*\*\*\*แล้วเลือก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="7aaf9-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="7aaf9-111">เลือกใช่ เพื่ออนุญาตให้ Registry Editor เปลี่ยนแปลงอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="7aaf9-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="7aaf9-112">ใน Registry Editor ให้เพิ่มค่า DWORD ของ **EnableADAL** ที่มีการตั้งค่า **เป็น 0** ภายใต้ HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="7aaf9-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="7aaf9-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="7aaf9-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>