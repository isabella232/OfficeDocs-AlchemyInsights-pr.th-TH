---
title: ไม่สามารถเปิดใช้งาน Office ได้
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
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812591"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="e69d4-102">ไม่สามารถเปิดใช้งาน Office ได้</span><span class="sxs-lookup"><span data-stu-id="e69d4-102">Unable to activate Office</span></span>

- <span data-ttu-id="e69d4-103">ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="e69d4-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="e69d4-104">ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตสิทธิ์การใช้งานไคลเอ็นต์ เช่น Office 365 Business หรือ Business Premium และตรวจสอบ[ให้แน่ใจว่าผู้ใช้ได้รับการมอบหมายสิทธิ์การใช้งาน](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="e69d4-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="e69d4-105">ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้ Office ด้วยบัญชีเดียวกันกับที่ได้รับการมอบหมายสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e69d4-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="e69d4-106">ตรวจสอบ [หน้า สถานภาพบริการของ Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) เพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="e69d4-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="e69d4-107">ตรวจสอบการตั้งค่าไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกไม่ให้แอป Microsoft 365 เข้าถึงอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="e69d4-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="e69d4-108">โปรดดู[URL และช่วงที่อยู่ IP ของ Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL และช่วงที่อยู่ IP ของ Office 365")</span><span class="sxs-lookup"><span data-stu-id="e69d4-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="e69d4-109">**เคล็ดลับ** บนเครื่อง Windows เราสามารถวินิจฉัยและแก้ไขปัญหาการลงชื่อเข้าใช้ Office ทั่วไปหลายอย่างให้คุณโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="e69d4-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="e69d4-110">ดาวน์โหลดและเรียกใช้  **[ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SaRA-OfficeSignInScenario)** ของ Microsoft เพื่อใช้เครื่องมืออัตโนมัติของเรา</span><span class="sxs-lookup"><span data-stu-id="e69d4-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="e69d4-111">ใช้การแอคชันการแก้ไขปัญหาต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="e69d4-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="e69d4-112">เปิดแอป Office [แล้วลงชื่อ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="e69d4-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="e69d4-113">[ลบ](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)[แล้วมอบหมายสิทธิ์การใช้งาน](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)Office ใหม่[แล้วลงชื่อเข้าใช้ Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="e69d4-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="e69d4-114">เรียกใช้ [ตัวแก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="e69d4-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="e69d4-115">ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่</span><span class="sxs-lookup"><span data-stu-id="e69d4-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่")
- [<span data-ttu-id="e69d4-116">ซ่อมแซมแบบออนไลน์ของ Office</span><span class="sxs-lookup"><span data-stu-id="e69d4-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="e69d4-117">ดูวิธีแก้ไขปัญหาเพิ่มเติมที่:</span><span class="sxs-lookup"><span data-stu-id="e69d4-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="e69d4-118">ข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาตและการเปิดใช้งานใน Office</span><span class="sxs-lookup"><span data-stu-id="e69d4-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="e69d4-119">"ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง" ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="e69d4-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)