---
title: ไม่สามารถเปิดใช้งาน Office ได้
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
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704949"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="62523-102">ไม่สามารถเปิดใช้งาน Office ได้</span><span class="sxs-lookup"><span data-stu-id="62523-102">Unable to activate Office</span></span>

- <span data-ttu-id="62523-103">ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="62523-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="62523-104">ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตสิทธิ์การใช้งานของลูกค้า เช่น Office 365 Business หรือ Business Premium และตรวจสอบ [ให้แน่ใจว่าผู้ใช้ได้รับการมอบหมาย](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)สิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="62523-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="62523-105">ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้ Office ด้วยบัญชีเดียวกันกับที่ได้รับการมอบหมายสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="62523-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="62523-106">ตรวจสอบ [หน้าสถานภาพบริการ Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) เพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="62523-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="62523-107">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าพวกเขาไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตของแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="62523-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="62523-108">โปรดดู[URL และช่วงที่อยู่ IP ของ Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL และช่วงที่อยู่ IP ของ Office 365")</span><span class="sxs-lookup"><span data-stu-id="62523-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="62523-109">**เคล็ดลับ** บนเครื่อง Windows เราสามารถวินิจฉัยและแก้ไขปัญหาการลงชื่อเข้าใช้ Office ทั่วไปหลายๆ อย่างให้คุณโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="62523-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="62523-110">ดาวน์โหลดและเรียกใช้  **[ตัวช่วยการสนับสนุนและการกู้คืนของ Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** เพื่อใช้เครื่องมืออัตโนมัติของเรา</span><span class="sxs-lookup"><span data-stu-id="62523-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="62523-111">ใช้การแก้ไขปัญหาต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="62523-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="62523-112">เปิดแอป Office [และ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ลงชื่อออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="62523-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="62523-113">[เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)[และกําหนดสิทธิ์การใช้งาน](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)Office ใหม่[แล้วลงชื่อเข้าใช้ Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="62523-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="62523-114">เรียกใช้ [ตัวแก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="62523-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="62523-115">รีเซ็ตสถานะการเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="62523-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "รีเซ็ตสถานะการเปิดใช้งาน Office")
- [<span data-ttu-id="62523-116">ซ่อมแซมแบบออนไลน์ของ Office</span><span class="sxs-lookup"><span data-stu-id="62523-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="62523-117">ดูวิธีแก้ไขปัญหาเพิ่มเติมที่:</span><span class="sxs-lookup"><span data-stu-id="62523-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="62523-118">ข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาตและการเปิดใช้งานใน Office</span><span class="sxs-lookup"><span data-stu-id="62523-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="62523-119">"ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง" ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="62523-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)