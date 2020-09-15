---
title: การลดการใช้แอปพลิเคชันไม่พบข้อผิดพลาด
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666997"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="8324c-102">เกิดข้อผิดพลาด "ไม่พบแอปพลิเคชัน"</span><span class="sxs-lookup"><span data-stu-id="8324c-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="8324c-103">ข้อผิดพลาดการติดตั้งแอป "ไม่พบแอปพลิเคชันหลังจากการติดตั้งเสร็จสมบูรณ์" รายงานโดย Intune อาจเกิดขึ้นบนแพลตฟอร์มระบบปฏิบัติการหลักทั้งหมด (Windows, iOS และ Android)</span><span class="sxs-lookup"><span data-stu-id="8324c-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="8324c-104">สถานการณ์สมมติทั่วไปส่วนใหญ่ที่สร้างข้อผิดพลาดนี้มีดังนี้</span><span class="sxs-lookup"><span data-stu-id="8324c-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="8324c-105">แอปที่ได้รับการอัปเดตที่อยู่ภายนอก Intune (จากที่เก็บแอปของบริษัทอื่น) หลังจากการปรับใช้ครั้งแรก</span><span class="sxs-lookup"><span data-stu-id="8324c-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="8324c-106">ตัวอย่างเช่นแอปพลิเคชันบางอย่างเช่น Google Chrome อาจดำเนินการอัปเดตอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="8324c-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="8324c-107">ผู้ใช้ได้ถอนการติดตั้งแอปหลังจากการติดตั้งเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="8324c-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="8324c-108">เมื่อต้องการลดปัญหานี้ก่อนอื่นให้ดำเนินการรีวิวอุปกรณ์ที่ได้รับผลกระทบเพื่อระบุสถานการณ์ที่เกิดข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="8324c-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="8324c-109">ถ้าแอปที่ได้รับการอัปเดตที่อยู่นอก Intune การปรับใช้แอปจะสามารถตั้งค่าให้ละเว้นเวอร์ชันของแอปพลิเคชันได้</span><span class="sxs-lookup"><span data-stu-id="8324c-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="8324c-110">เมื่อต้องการทำเช่นนั้นภายใต้**การกำหนดค่าแอป > ข้อมูลแอป**ให้ตั้งค่าละเว้นเวอร์ชันของ**แอป**เป็น**ใช่**</span><span class="sxs-lookup"><span data-stu-id="8324c-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="8324c-111">เมื่อกำหนดเป้าหมายไคลเอ็นต์อาจเหมาะสมที่จะปรับใช้แอปพลิเคชันเป็น "จำเป็น" และเพื่อให้แน่ใจว่ามีการปรับใช้เวอร์ชันล่าสุด</span><span class="sxs-lookup"><span data-stu-id="8324c-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="8324c-112">อีกวิธีหนึ่งคือบนแพลตฟอร์ม iOS คุณสามารถใช้ฟังก์ชันการทำงาน **autoupdate** ที่เกี่ยวข้องกับโปรแกรมการซื้อปริมาณ Apple ซึ่งสามารถกำหนดค่าให้อัปเดตเป็นเวอร์ชันแอปพลิเคชันใหม่ได้โดยอัตโนมัติเมื่อพร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="8324c-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="8324c-113">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการแก้ไขปัญหาการติดตั้งแอปโปรดดูที่[แก้ไขปัญหาการติดตั้งแอป](https://docs.microsoft.com/intune/troubleshoot-app-install)</span><span class="sxs-lookup"><span data-stu-id="8324c-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
