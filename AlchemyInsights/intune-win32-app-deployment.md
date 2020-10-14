---
title: การปรับใช้แอป Intune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461995"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="2679b-102">การปรับใช้แอป Intune Win32</span><span class="sxs-lookup"><span data-stu-id="2679b-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="2679b-103">Microsoft Intune ช่วยให้แอปพลิเคชัน Win32 รวมถึงแต่ไม่จำกัดเฉพาะ MSI และ EXE ของคุณสามารถปรับใช้กับอุปกรณ์ Windows 10 ได้</span><span class="sxs-lookup"><span data-stu-id="2679b-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="2679b-104">กลไกการปรับใช้ที่ใช้จำเป็นต้องมีส่วนขยายการจัดการ Intune (IME) ที่จะนำเสนอบนอุปกรณ์เป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="2679b-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="2679b-105">IME จะได้รับการติดตั้งโดยอัตโนมัติเป็นผลลัพธ์ของการกำหนดเป้าหมายสคริปต์ powershell หรือการปรับใช้แอปพลิเคชัน win32 กับผู้ใช้/อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="2679b-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="2679b-106">นอกจากนี้ยังมีชุดของ requisites ที่ต้องตรงตามลำดับเพื่อปรับใช้แอปพลิเคชัน Win32 ซึ่งรวมถึง:</span><span class="sxs-lookup"><span data-stu-id="2679b-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="2679b-107">แพลตฟอร์มที่ได้รับการสนับสนุน: Windows 10 เวอร์ชัน๑๖๐๗หรือเวอร์ชันที่ใหม่กว่า (Enterprise, Pro และการศึกษา)</span><span class="sxs-lookup"><span data-stu-id="2679b-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="2679b-108">สถาปัตยกรรมที่ได้รับการสนับสนุน: x86 และ x64</span><span class="sxs-lookup"><span data-stu-id="2679b-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="2679b-109">การจัดการอุปกรณ์: AAD เข้าร่วมและลงทะเบียนโดยอัตโนมัติ (รวมถึงการเข้าร่วมโดเมนแบบไฮบริดและการลงทะเบียนนโยบายกลุ่มโดยอัตโนมัติ)</span><span class="sxs-lookup"><span data-stu-id="2679b-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="2679b-110">รูปแบบแพคเกจแอปพลิเคชัน: ไฟล์**intunewin**ที่เตรียมโดย[เครื่องมือการเตรียมเนื้อหาของ Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)</span><span class="sxs-lookup"><span data-stu-id="2679b-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="2679b-111">ข้อจำกัด</span><span class="sxs-lookup"><span data-stu-id="2679b-111">Limitations:</span></span>
    - <span data-ttu-id="2679b-112">ขนาดสูงสุด: 8GB</span><span class="sxs-lookup"><span data-stu-id="2679b-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="2679b-113">สถาปัตยกรรมที่ไม่ได้รับการสนับสนุน: แขน</span><span class="sxs-lookup"><span data-stu-id="2679b-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="2679b-114">ตรวจทานเอกสาร "[เพิ่มมอบหมายและตรวจสอบแอป Win32 ใน Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" สำหรับข้อมูลที่เกี่ยวข้องกับขั้นตอนเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="2679b-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="2679b-115">รายละเอียดเกี่ยวกับการแก้ไขปัญหาการปรับใช้แอปพลิเคชันบน Windows รวมถึงแอป Win32 ที่สามารถรีวิวได้ในเอกสารต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="2679b-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="2679b-116">แก้ไขปัญหาการติดตั้งแอป</span><span class="sxs-lookup"><span data-stu-id="2679b-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="2679b-117">การแก้ปัญหาแอป Win32</span><span class="sxs-lookup"><span data-stu-id="2679b-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)