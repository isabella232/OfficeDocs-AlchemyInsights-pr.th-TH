---
title: ติดตั้งเซิร์ฟเวอร์รายงาน Power BI
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
- "1304"
- "2500001"
ms.openlocfilehash: 3ea596547093773ab872ca34e8dd3a4e49e59fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755114"
---
# <a name="install-power-bi-report-server"></a><span data-ttu-id="2b87e-102">ติดตั้งเซิร์ฟเวอร์รายงาน Power BI</span><span class="sxs-lookup"><span data-stu-id="2b87e-102">Install Power BI Report Server</span></span>

1. <span data-ttu-id="2b87e-103">ค้นหาตำแหน่งที่ตั้งของ PowerBIReportServer.exe และเปิดใช้งานตัวติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="2b87e-103">Find the location of PowerBIReportServer.exe and launch the installer.</span></span>

2. <span data-ttu-id="2b87e-104">เลือก**ติดตั้งเซิร์ฟเวอร์รายงาน POWER BI**</span><span class="sxs-lookup"><span data-stu-id="2b87e-104">Select **Install Power BI Report Server**.</span></span>

3. <span data-ttu-id="2b87e-105">เลือกรุ่นที่ต้องการติดตั้งแล้วเลือก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="2b87e-105">Choose an edition to install and then select **Next**.</span></span>

4. <span data-ttu-id="2b87e-106">คุณสามารถเลือกการประเมินหรือรุ่นสำหรับนักพัฒนาจากดรอปดาวน์ได้</span><span class="sxs-lookup"><span data-stu-id="2b87e-106">You can choose either Evaluation or Developer edition from the drop down.</span></span>  <span data-ttu-id="2b87e-107">มิฉะนั้นคุณสามารถใส่คีย์ผลิตภัณฑ์สำหรับเซิร์ฟเวอร์ที่คุณได้รับจากบริการ Power BI หรือศูนย์บริการ Volume License</span><span class="sxs-lookup"><span data-stu-id="2b87e-107">Otherwise, you can enter a product key for the server that you acquired from either the Power BI service or the Volume License Service Center.</span></span> <span data-ttu-id="2b87e-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการรับคีย์ผลิตภัณฑ์ของคุณให้ดูที่ส่วนก่อนที่คุณจะเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="2b87e-108">For more information about how to get your product key, see the Before you begin section.</span></span> <span data-ttu-id="2b87e-109">อ่านและยอมรับข้อกำหนดและเงื่อนไขสิทธิ์การใช้งานแล้วเลือก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="2b87e-109">Read and agree to the license terms and conditions, and then select **Next**.</span></span>

5. <span data-ttu-id="2b87e-110">คุณจำเป็นต้องมีกลไกจัดการฐานข้อมูลที่พร้อมใช้งานสำหรับการจัดเก็บฐานข้อมูลเซิร์ฟเวอร์รายงาน</span><span class="sxs-lookup"><span data-stu-id="2b87e-110">You need to have a Database Engine available to store the report server database.</span></span> <span data-ttu-id="2b87e-111">เลือก **ถัด** ไปเพื่อติดตั้งเซิร์ฟเวอร์รายงานเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="2b87e-111">Select **Next** to install the report server only.</span></span>

6. <span data-ttu-id="2b87e-112">ระบุตำแหน่งที่ตั้งติดตั้งสำหรับเซิร์ฟเวอร์รายงาน</span><span class="sxs-lookup"><span data-stu-id="2b87e-112">Specify the install location for the report server.</span></span> <span data-ttu-id="2b87e-113">เลือก **ติดตั้ง** เพื่อดำเนินการต่อ</span><span class="sxs-lookup"><span data-stu-id="2b87e-113">Select **Install** to continue.</span></span>

7. <span data-ttu-id="2b87e-114">หลังจากการตั้งค่าที่เสร็จสมบูรณ์แล้วให้เลือก **กำหนดค่าเซิร์ฟเวอร์รายงาน** เพื่อเปิดใช้งานตัวจัดการการตั้งค่าคอนฟิกของบริการรายงาน</span><span class="sxs-lookup"><span data-stu-id="2b87e-114">After a successful setup, select **Configure Report Server** to launch the Reporting Services Configuration Manager.</span></span>

<span data-ttu-id="2b87e-115">คุณไม่จำเป็นต้องมีเซิร์ฟเวอร์โปรแกรมฐานข้อมูล SQL Server ที่พร้อมใช้งานในขณะที่ติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="2b87e-115">You don't need a SQL Server Database Engine server available at the time of install.</span></span> <span data-ttu-id="2b87e-116">คุณจะต้องมีหนึ่งเพื่อกำหนดค่าบริการการรายงานหลังจากติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="2b87e-116">You will need one to configure Reporting Services after install.</span></span>

<span data-ttu-id="2b87e-117">สำหรับข้อมูลเพิ่มเติม: https://docs.microsoft.com/power-bi/report-server/install-report-server</span><span class="sxs-lookup"><span data-stu-id="2b87e-117">For more information: https://docs.microsoft.com/power-bi/report-server/install-report-server</span></span>
