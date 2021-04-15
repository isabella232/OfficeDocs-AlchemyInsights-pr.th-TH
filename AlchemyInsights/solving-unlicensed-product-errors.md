---
title: การแก้ไขปัญหาข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาต
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
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786868"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="04f03-102">ข้อเสนอแนะเพื่อแก้ไขข้อผิดพลาด "ผลิตภัณฑ์ที่ไม่มีใบอนุญาต"</span><span class="sxs-lookup"><span data-stu-id="04f03-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="04f03-103">เมื่อต้องการแก้ไขข้อผิดพลาดเกี่ยวกับ "ผลิตภัณฑ์ที่ไม่มีใบอนุญาต" ให้ลองใช้วิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="04f03-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="04f03-104">ตรวจสอบเพื่อดูว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="04f03-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="04f03-105">ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตสิทธิ์การใช้งานไคลเอ็นต์ เช่น แอป Microsoft 365 For Business หรือ Business Premium และตรวจสอบให้แน่ใจว่า [ผู้ใช้ได้รับการมอบหมาย](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)สิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="04f03-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="04f03-106">ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้ Office ด้วยบัญชีเดียวกันกับที่ได้รับการมอบหมายสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="04f03-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="04f03-107">ตรวจสอบ [หน้า สถานภาพ](https://docs.microsoft.com/office365/enterprise/view-service-health) บริการ เพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="04f03-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="04f03-108">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกไม่ให้แอป Microsoft 365 เข้าถึงอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="04f03-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="04f03-109">ดู [URL และช่วงที่อยู่](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)IP</span><span class="sxs-lookup"><span data-stu-id="04f03-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="04f03-110">คุณอาจลองแก้ไขปัญหาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="04f03-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="04f03-111">เปิดแอป Office [แล้วลงชื่อ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="04f03-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="04f03-112">[เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)[และกําหนด](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)สิทธิ์การใช้งาน Office ใหม่[แล้วลงชื่อเข้าใช้ Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="04f03-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="04f03-113">เรียกใช้ [ตัวแก้ไขปัญหา](https://aka.ms/SARA-OfficeActivation-Alchemy)การเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="04f03-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="04f03-114">[รีเซ็ตสถานะการเปิดใช้งาน Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="04f03-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="04f03-115">[ซ่อมแซมแบบออนไลน์ของ Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="04f03-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="04f03-116">ดูวิธีแก้ไขปัญหาเพิ่มเติมที่:</span><span class="sxs-lookup"><span data-stu-id="04f03-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="04f03-117">ข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาตและการเปิดใช้งานใน Office</span><span class="sxs-lookup"><span data-stu-id="04f03-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="04f03-118">"ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง" ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="04f03-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)