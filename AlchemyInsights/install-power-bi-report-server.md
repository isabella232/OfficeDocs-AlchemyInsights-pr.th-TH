---
title: ติดตั้งเซิร์ฟเวอร์รายงาน BI พลังงาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 38ef162bd5c26328ee70af37df07adfbf2bfd93b
ms.sourcegitcommit: e17e7d17fdb638349bb320b318085138d18f284c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2019
ms.locfileid: "35752394"
---
# <a name="install-power-bi-report-server"></a><span data-ttu-id="5d673-102">ติดตั้งเซิร์ฟเวอร์รายงาน BI พลังงาน</span><span class="sxs-lookup"><span data-stu-id="5d673-102">Install Power BI Report Server</span></span>

1. <span data-ttu-id="5d673-103">ค้นหาตำแหน่งที่ตั้งของ PowerBIReportServer.exe และเรียกใช้โปรแกรมติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="5d673-103">Find the location of PowerBIReportServer.exe and launch the installer.</span></span>

2. <span data-ttu-id="5d673-104">เลือกการ**ติดตั้งเซิร์ฟเวอร์รายงาน BI พลังงาน**</span><span class="sxs-lookup"><span data-stu-id="5d673-104">Select **Install Power BI Report Server**.</span></span>

3. <span data-ttu-id="5d673-105">เลือกรุ่นที่ติดตั้ง และจากนั้น เลือก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="5d673-105">Choose an edition to install and then select **Next**.</span></span>

4. <span data-ttu-id="5d673-106">คุณสามารถเลือกรุ่นทดลองหรือนักพัฒนาจากแบบหล่นลง</span><span class="sxs-lookup"><span data-stu-id="5d673-106">You can choose either Evaluation or Developer edition from the drop down.</span></span>  <span data-ttu-id="5d673-107">มิฉะนั้น คุณสามารถป้อนหมายเลขผลิตภัณฑ์สำหรับเซิร์ฟเวอร์ที่คุณซื้อมาจากบริการ BI พลังงานหรือศูนย์บริการสิทธิ์การใช้งานไดรฟ์ข้อมูล</span><span class="sxs-lookup"><span data-stu-id="5d673-107">Otherwise, you can enter a product key for the server that you acquired from either the Power BI service or the Volume License Service Center.</span></span> <span data-ttu-id="5d673-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการเรียกดูของคุณ คีย์ผลิตภัณฑ์ Before คุณเริ่มต้นส่วน</span><span class="sxs-lookup"><span data-stu-id="5d673-108">For more information about how to get your product key, see the Before you begin section.</span></span> <span data-ttu-id="5d673-109">อ่าน และยอมรับเงื่อนไขการอนุญาตให้ใช้สิทธิและเงื่อนไข และจากนั้น เลือก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="5d673-109">Read and agree to the license terms and conditions, and then select **Next**.</span></span>

5. <span data-ttu-id="5d673-110">คุณจำเป็นต้องมีกลไกจัดการฐานข้อมูลพร้อมใช้งานในการจัดเก็บในฐานข้อมูลเซิร์ฟเวอร์รายงาน</span><span class="sxs-lookup"><span data-stu-id="5d673-110">You need to have a Database Engine available to store the report server database.</span></span> <span data-ttu-id="5d673-111">เลือก**ถัดไป**เพื่อติดตั้งเซิร์ฟเวอร์รายงานเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="5d673-111">Select **Next** to install the report server only.</span></span>

6. <span data-ttu-id="5d673-112">ระบุตำแหน่งการติดตั้งสำหรับเซิร์ฟเวอร์รายงาน</span><span class="sxs-lookup"><span data-stu-id="5d673-112">Specify the install location for the report server.</span></span> <span data-ttu-id="5d673-113">เลือกการ**ติดตั้ง**เพื่อดำเนินต่อ</span><span class="sxs-lookup"><span data-stu-id="5d673-113">Select **Install** to continue.</span></span>

7. <span data-ttu-id="5d673-114">หลังจากตั้งค่าเสร็จเรียบร้อยแล้ว เลือกการ**ตั้งค่าคอนฟิกเซิร์ฟเวอร์รายงาน**ที่จะเปิดใช้โปรแกรมจัดการการตั้งค่าคอนฟิกบริการรายงาน</span><span class="sxs-lookup"><span data-stu-id="5d673-114">After a successful setup, select **Configure Report Server** to launch the Reporting Services Configuration Manager.</span></span>

<span data-ttu-id="5d673-115">คุณไม่ต้องการเซิร์ฟเวอร์ SQL Server Database Engine ที่พร้อมใช้งาน ณเวลาติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="5d673-115">You don't need a SQL Server Database Engine server available at the time of install.</span></span> <span data-ttu-id="5d673-116">คุณจะต้องการตั้งค่าคอนฟิกบริการรายงานหลังจากการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="5d673-116">You will need one to configure Reporting Services after install.</span></span>

<span data-ttu-id="5d673-117">สำหรับข้อมูลเพิ่มเติม:https://docs.microsoft.com/power-bi/report-server/install-report-server</span><span class="sxs-lookup"><span data-stu-id="5d673-117">For more information: https://docs.microsoft.com/power-bi/report-server/install-report-server</span></span>
