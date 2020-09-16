---
title: การแก้ไขข้อผิดพลาดของผลิตภัณฑ์ที่ไม่มีสิทธิ์
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737972"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="b9fd7-102">ข้อเสนอแนะสำหรับการแก้ไขข้อผิดพลาด "ผลิตภัณฑ์ที่ไม่มีสิทธิ์"</span><span class="sxs-lookup"><span data-stu-id="b9fd7-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="b9fd7-103">เมื่อต้องการแก้ไขข้อผิดพลาดเกี่ยวกับ "ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งาน" ให้ลองดำเนินการดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="b9fd7-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="b9fd7-104">ตรวจสอบดูว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="b9fd7-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="b9fd7-105">ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตให้ใช้สิทธิ์การใช้งานไคลเอ็นต์เช่น Microsoft ๓๖๕ Apps for business หรือ Business Premium และ [ตรวจสอบให้แน่ใจว่าผู้ใช้มีสิทธิ์](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)การใช้งานที่ได้รับมอบหมาย</span><span class="sxs-lookup"><span data-stu-id="b9fd7-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="b9fd7-106">ตรวจสอบให้แน่ใจว่าผู้ใช้กำลังลงชื่อเข้าใช้ Office ด้วยบัญชีผู้ใช้เดียวกันกับสิทธิ์การใช้งานที่ได้รับมอบหมาย</span><span class="sxs-lookup"><span data-stu-id="b9fd7-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="b9fd7-107">ตรวจสอบ [หน้าสถานภาพบริการ](https://docs.microsoft.com/office365/enterprise/view-service-health) เพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="b9fd7-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="b9fd7-108">ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าพวกเขาไม่ได้บล็อก Microsoft ๓๖๕ apps access ไปยังอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="b9fd7-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="b9fd7-109">ให้ดู[ที่ url และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="b9fd7-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="b9fd7-110">นอกจากนี้คุณอาจลองการดำเนินการแก้ไขปัญหาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b9fd7-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="b9fd7-111">เปิดแอป Office และ [ลงชื่อออกจาก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) บัญชีผู้ใช้ใดๆที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="b9fd7-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="b9fd7-112">[เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) และกำหนดสิทธิ์การใช้งาน Office [อีกครั้ง](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) แล้ว [ลงชื่อเข้าใช้ office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="b9fd7-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="b9fd7-113">เรียกใช้ตัว[แก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="b9fd7-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="b9fd7-114">[ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="b9fd7-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="b9fd7-115">[ดำเนินการซ่อมแซมแบบออนไลน์ของ Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="b9fd7-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="b9fd7-116">สำหรับโซลูชันการแก้ไขปัญหาเพิ่มเติมให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="b9fd7-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="b9fd7-117">ข้อผิดพลาดในการเปิดใช้งานผลิตภัณฑ์และการเปิดใช้งานใน Office</span><span class="sxs-lookup"><span data-stu-id="b9fd7-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="b9fd7-118">"ขออภัยเราไม่สามารถเชื่อมต่อกับบัญชีผู้ใช้ของคุณได้ โปรดลองอีกครั้งในภายหลัง "ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="b9fd7-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)