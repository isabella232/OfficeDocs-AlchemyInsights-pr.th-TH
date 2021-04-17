---
title: ติดตั้งเซิร์ฟเวอร์รายงาน Power BI
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 8479be2a538228b71033aca3907d3aba2f5e28fb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832113"
---
# <a name="install-power-bi-report-server"></a><span data-ttu-id="910a7-102">ติดตั้งเซิร์ฟเวอร์รายงาน Power BI</span><span class="sxs-lookup"><span data-stu-id="910a7-102">Install Power BI Report Server</span></span>

1. <span data-ttu-id="910a7-103">ค้นหาสถานที่ของPowerBIReportServer.exe และเรียกใช้ตัวติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="910a7-103">Find the location of PowerBIReportServer.exe and launch the installer.</span></span>

2. <span data-ttu-id="910a7-104">เลือก **ติดตั้งเซิร์ฟเวอร์รายงาน Power** BI</span><span class="sxs-lookup"><span data-stu-id="910a7-104">Select **Install Power BI Report Server**.</span></span>

3. <span data-ttu-id="910a7-105">เลือกรุ่นที่จะติดตั้ง **แล้วเลือก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="910a7-105">Choose an edition to install and then select **Next**.</span></span>

4. <span data-ttu-id="910a7-106">คุณสามารถเลือกรุ่นการประเมินหรือนักพัฒนาได้จากเมนูดรอปดาวน์</span><span class="sxs-lookup"><span data-stu-id="910a7-106">You can choose either Evaluation or Developer edition from the drop down.</span></span>  <span data-ttu-id="910a7-107">มิฉะนั้น คุณสามารถใส่คีย์ผลิตภัณฑ์ของเซิร์ฟเวอร์ที่คุณซื้อจากบริการ Power BI หรือศูนย์บริการ Volume License</span><span class="sxs-lookup"><span data-stu-id="910a7-107">Otherwise, you can enter a product key for the server that you acquired from either the Power BI service or the Volume License Service Center.</span></span> <span data-ttu-id="910a7-108">หากต้องการข้อมูลเพิ่มเติมเกี่ยวกับวิธีการรับคีย์ผลิตภัณฑ์ของคุณ ให้ดูที่ส่วน ก่อนที่คุณจะเริ่ม</span><span class="sxs-lookup"><span data-stu-id="910a7-108">For more information about how to get your product key, see the Before you begin section.</span></span> <span data-ttu-id="910a7-109">อ่านและยอมรับข้อกวมและเงื่อนไขของสิทธิ์การใช้งาน **จากนั้นเลือก** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="910a7-109">Read and agree to the license terms and conditions, and then select **Next**.</span></span>

5. <span data-ttu-id="910a7-110">คุณจึงต้องมีกลไกจัดการฐานข้อมูลที่พร้อมให้ใช้งานเพื่อจัดเก็บฐานข้อมูลเซิร์ฟเวอร์รายงาน</span><span class="sxs-lookup"><span data-stu-id="910a7-110">You need to have a Database Engine available to store the report server database.</span></span> <span data-ttu-id="910a7-111">เลือกถัดไป เพื่อติดตั้งเซิร์ฟเวอร์รายงานเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="910a7-111">Select **Next** to install the report server only.</span></span>

6. <span data-ttu-id="910a7-112">ระบุที่ตั้งการติดตั้งเซิร์ฟเวอร์รายงาน</span><span class="sxs-lookup"><span data-stu-id="910a7-112">Specify the install location for the report server.</span></span> <span data-ttu-id="910a7-113">เลือก **ติดตั้ง เพื่อ** ใช้งานต่อ</span><span class="sxs-lookup"><span data-stu-id="910a7-113">Select **Install** to continue.</span></span>

7. <span data-ttu-id="910a7-114">หลังจากการตั้งค่าเสร็จเรียบร้อยแล้ว ให้เลือก **กําหนดค่าเซิร์ฟเวอร์** รายงาน เพื่อเปิดใช้ตัวจัดการการกําหนดค่า Reporting Services</span><span class="sxs-lookup"><span data-stu-id="910a7-114">After a successful setup, select **Configure Report Server** to launch the Reporting Services Configuration Manager.</span></span>

<span data-ttu-id="910a7-115">คุณไม่ต้องใช้เซิร์ฟเวอร์ SQL Server Database Engine ที่พร้อมใช้งานเมื่อติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="910a7-115">You don't need a SQL Server Database Engine server available at the time of install.</span></span> <span data-ttu-id="910a7-116">คุณจะต้องใช้เพื่อกําหนดค่า Reporting Services หลังจากติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="910a7-116">You will need one to configure Reporting Services after install.</span></span>

<span data-ttu-id="910a7-117">For more information: https://docs.microsoft.com/power-bi/report-server/install-report-server</span><span class="sxs-lookup"><span data-stu-id="910a7-117">For more information: https://docs.microsoft.com/power-bi/report-server/install-report-server</span></span>
