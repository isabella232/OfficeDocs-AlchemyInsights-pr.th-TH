---
title: ลดข้อผิดพลาด แอปพลิเคชันไม่พบข้อผิดพลาด
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836370"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="de415-102">แก้ไขข้อผิดพลาด "ไม่พบแอปพลิเคชัน"</span><span class="sxs-lookup"><span data-stu-id="de415-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="de415-103">ข้อผิดพลาดการติดตั้งแอป "ไม่พบแอปพลิเคชันหลังจากการติดตั้งเสร็จสมบูรณ์" ที่รายงานโดย Intun1 อาจเกิดขึ้นบนแพลตฟอร์ม OS หลักทั้งหมด (Windows, iOS และ Android)</span><span class="sxs-lookup"><span data-stu-id="de415-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="de415-104">สถานการณ์ทั่วไปที่สร้างข้อผิดพลาดนี้ ได้แก่</span><span class="sxs-lookup"><span data-stu-id="de415-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="de415-105">แอปได้รับการอัปเดตภายนอก Intun1 (จากร้านค้าแอปของบริษัทอื่น) หลังจากการปรับใช้ครั้งแรก</span><span class="sxs-lookup"><span data-stu-id="de415-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="de415-106">ตัวอย่างเช่น บางแอปพลิเคชัน เช่น Google Chrome อาจอัปเดตโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="de415-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="de415-107">ผู้ใช้ถอนการติดตั้งแอปหลังจากการติดตั้งครั้งแรก</span><span class="sxs-lookup"><span data-stu-id="de415-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="de415-108">เมื่อต้องการลดปัญหานี้ ก่อนอื่นให้ตรวจสอบอุปกรณ์ที่ได้รับผลกระทบเพื่อระบุสถานการณ์ที่ข้อผิดพลาดเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="de415-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="de415-109">ถ้าแอปได้รับการอัปเดตภายนอก Intun1 สามารถตั้งค่าการปรับใช้แอปให้ละเว้นเวอร์ชันของแอปพลิเคชันได้</span><span class="sxs-lookup"><span data-stu-id="de415-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="de415-110">To do so, under **App Configuration > App Information**, set Ignore **App** version to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="de415-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="de415-111">เมื่อ targeting the client, it may be appropriate to deploy the application as "required," and to ensure that the latest version is deployed.</span><span class="sxs-lookup"><span data-stu-id="de415-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="de415-112">หรือ บนแพลตฟอร์ม iOS คุณสามารถใช้ฟังก์ชัน **autoupdate** ที่เกี่ยวข้องกับโปรแกรมการซื้อของ Apple ซึ่งสามารถกําหนดค่าให้อัปเดตเป็นแอปพลิเคชันเวอร์ชันใหม่โดยอัตโนมัติเมื่อพร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="de415-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="de415-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation](https://docs.microsoft.com/intune/troubleshoot-app-install)issues .</span><span class="sxs-lookup"><span data-stu-id="de415-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
