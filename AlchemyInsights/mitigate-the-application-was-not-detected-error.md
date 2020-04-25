---
title: ลดปัญหา
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810502"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="eb14e-102">ลดข้อผิดพลาด "โปรแกรมประยุกต์ไม่พบ"</span><span class="sxs-lookup"><span data-stu-id="eb14e-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="eb14e-103">ข้อผิดพลาดการติดตั้งแอป "โปรแกรมประยุกต์ไม่พบหลังจากการติดตั้งเสร็จสมบูรณ์" รายงานโดย Intune อาจเกิดขึ้นบนแพลตฟอร์มระบบปฏิบัติการหลักทั้งหมด (Windows, iOS และ Android)</span><span class="sxs-lookup"><span data-stu-id="eb14e-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="eb14e-104">สถานการณ์ทั่วไปที่ทําให้เกิดข้อผิดพลาดนี้รวมถึง:</span><span class="sxs-lookup"><span data-stu-id="eb14e-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="eb14e-105">แอปได้รับการปรับปรุงภายนอก Intune (จากร้านค้าแอปของบริษัทอื่น)</span><span class="sxs-lookup"><span data-stu-id="eb14e-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="eb14e-106">ตัวอย่างเช่นแอปพลิเคชันบางอย่างเช่น Google Chrome อาจดําเนินการอัปเดตอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="eb14e-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="eb14e-107">ผู้ใช้ได้ถอนการติดตั้งแอปหลังจากการติดตั้งครั้งแรก</span><span class="sxs-lookup"><span data-stu-id="eb14e-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="eb14e-108">เมื่อต้องการลดปัญหานี้ ก่อนทําการตรวจสอบอุปกรณ์ที่ได้รับผลกระทบเพื่อกําหนดสถานการณ์ที่เกิดข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="eb14e-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="eb14e-109">ถ้าโปรแกรมประยุกต์ได้รับการปรับปรุงภายนอก Intune การปรับใช้โปรแกรมประยุกต์สามารถตั้งค่าให้ละเว้นเวอร์ชันของแอพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="eb14e-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="eb14e-110">เมื่อต้องการดําเนินการดังกล่าว ภายใต้**การกําหนดค่าแอป > ข้อมูลแอป**ให้ตั้งค่า**ละเว้นเวอร์ชันของแอป**เป็น**ใช่**</span><span class="sxs-lookup"><span data-stu-id="eb14e-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="eb14e-111">เมื่อกําหนดเป้าหมายไคลเอนต์ อาจเหมาะสมในการปรับใช้โปรแกรมประยุกต์เป็น "จําเป็น" และเพื่อให้แน่ใจว่า มีการปรับใช้รุ่นล่าสุด</span><span class="sxs-lookup"><span data-stu-id="eb14e-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="eb14e-112">อีกทางเลือกหนึ่ง, บนแพลตฟอร์ม iOS, มันเป็นไปได้ที่จะใช้ฟังก์ชัน**autoupdate**ที่เกี่ยวข้องกับโปรแกรมการซื้อปริมาณแอปเปิ้ล, ซึ่งสามารถกําหนดค่าให้โดยอัตโนมัติอัปเดตเป็นเวอร์ชันของโปรแกรมประยุกต์ใหม่ที่พวกเขากลายเป็นใช้ได้.</span><span class="sxs-lookup"><span data-stu-id="eb14e-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="eb14e-113">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการแก้ไขปัญหาการติดตั้งแอป โปรดดู[แก้ไขปัญหาการติดตั้งแอป](https://docs.microsoft.com/intune/troubleshoot-app-install)</span><span class="sxs-lookup"><span data-stu-id="eb14e-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
