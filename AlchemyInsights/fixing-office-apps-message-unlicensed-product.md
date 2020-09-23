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
ms.openlocfilehash: e052c18eae035ff05c70a223f6d8a2eab875b2c9
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236108"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="31b5b-102">ไม่สามารถเปิดใช้งาน Office ได้</span><span class="sxs-lookup"><span data-stu-id="31b5b-102">Unable to activate Office</span></span>

- <span data-ttu-id="31b5b-103">ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="31b5b-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="31b5b-104">ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตให้ใช้สิทธิ์การใช้งานไคลเอ็นต์เช่น Office ๓๖๕ Business หรือ Business Premium และ [ตรวจสอบให้แน่ใจว่าผู้ใช้มีสิทธิ์](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users)การใช้งานที่ได้รับมอบหมาย</span><span class="sxs-lookup"><span data-stu-id="31b5b-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="31b5b-105">ตรวจสอบให้แน่ใจว่าผู้ใช้กำลังลงชื่อเข้าใช้ Office ด้วยบัญชีผู้ใช้เดียวกันกับสิทธิ์การใช้งานที่ได้รับมอบหมาย</span><span class="sxs-lookup"><span data-stu-id="31b5b-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="31b5b-106">ตรวจสอบ [หน้าสถานภาพบริการของ Office ๓๖๕](https://docs.microsoft.com/office365/enterprise/view-service-health) เพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="31b5b-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="31b5b-107">ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าพวกเขาไม่ได้บล็อก Microsoft ๓๖๕ apps access ไปยังอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="31b5b-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="31b5b-108">โปรดดู[ที่ url และช่วงที่อยู่ IP ของ Office ๓๖๕](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Url และช่วงที่อยู่ IP ของ Office ๓๖๕")</span><span class="sxs-lookup"><span data-stu-id="31b5b-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="31b5b-109">**เคล็ดลับ** บนเครื่อง Windows เราสามารถวินิจฉัยและแก้ไขปัญหาการลงชื่อเข้าใช้ Office ทั่วไปได้โดยอัตโนมัติสำหรับคุณ</span><span class="sxs-lookup"><span data-stu-id="31b5b-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="31b5b-110">ดาวน์โหลดและเรียกใช้ตัว  **[ช่วยการสนับสนุนและการกู้คืนของ Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** เพื่อใช้เครื่องมืออัตโนมัติของเรา</span><span class="sxs-lookup"><span data-stu-id="31b5b-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="31b5b-111">ใช้การดำเนินการแก้ไขปัญหาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="31b5b-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="31b5b-112">เปิดแอป Office และ [ลงชื่อออก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) จากบัญชีผู้ใช้ใดๆที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="31b5b-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="31b5b-113">[เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) และกำหนดสิทธิ์การใช้งาน Office [อีกครั้ง](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) แล้ว [ลงชื่อ](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) เข้าใช้ office โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="31b5b-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="31b5b-114">เรียกใช้ตัว [แก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="31b5b-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="31b5b-115">ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่</span><span class="sxs-lookup"><span data-stu-id="31b5b-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่")
- [<span data-ttu-id="31b5b-116">ดำเนินการซ่อมแซมแบบออนไลน์ของ Office</span><span class="sxs-lookup"><span data-stu-id="31b5b-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="31b5b-117">สำหรับโซลูชันการแก้ไขปัญหาเพิ่มเติมให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="31b5b-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="31b5b-118">ข้อผิดพลาดในการเปิดใช้งานผลิตภัณฑ์และการเปิดใช้งานใน Office</span><span class="sxs-lookup"><span data-stu-id="31b5b-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="31b5b-119">"ขออภัยเราไม่สามารถเชื่อมต่อกับบัญชีผู้ใช้ของคุณได้ โปรดลองอีกครั้งในภายหลัง "ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="31b5b-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)