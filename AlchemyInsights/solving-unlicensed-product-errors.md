---
title: การแก้ไขข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: b629f24014a789b1f9847f62e725f726d4199027
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512031"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="e94cd-102">คําแนะนําสําหรับการแก้ปัญหาข้อผิดพลาด "ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งาน"</span><span class="sxs-lookup"><span data-stu-id="e94cd-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="e94cd-103">เมื่อต้องการแก้ไขข้อผิดพลาดเกี่ยวกับ "ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งาน" ให้ลองทําดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="e94cd-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="e94cd-104">ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="e94cd-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="e94cd-105">ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตให้มีสิทธิ์การใช้งานไคลเอ็นต์ เช่น Microsoft 365 Apps สําหรับธุรกิจหรือ Business Premium และ[ตรวจสอบว่าผู้ใช้มีสิทธิ์การใช้งานที่ได้รับมอบหมาย](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="e94cd-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="e94cd-106">ตรวจสอบให้แน่ใจว่า ผู้ใช้ลงชื่อเข้าใช้ Office ด้วยบัญชีผู้ใช้เดียวกันกับที่มีการกําหนดสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e94cd-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="e94cd-107">ตรวจสอบ[หน้าสถานภาพบริการ](https://docs.microsoft.com/office365/enterprise/view-service-health)เพื่อดูว่ามีปัญหาใด ๆ ที่ทราบเกี่ยวกับบริการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="e94cd-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="e94cd-108">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าไฟร์วอลล์ไม่ได้บล็อกการเข้าถึงแอป Office ไปยังอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="e94cd-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Office apps access to the Internet.</span></span> <span data-ttu-id="e94cd-109">ดู[URL และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="e94cd-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="e94cd-110">นอกจากนี้คุณอาจลองการดําเนินการแก้ไขปัญหาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e94cd-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="e94cd-111">เปิดแอป Office และ[ออกจากระบบ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)บัญชีผู้ใช้ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="e94cd-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="e94cd-112">[เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)และมอบหมายสิทธิ์การใช้งาน Office[แล้ว](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)[เข้าสู่ระบบ Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="e94cd-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="e94cd-113">เรียกใช้[ตัวแก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="e94cd-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="e94cd-114">[รีเซ็ตสถานะการเปิดใช้งาน Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="e94cd-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="e94cd-115">[ดําเนินการซ่อมแซม Office แบบออนไลน์](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="e94cd-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="e94cd-116">สําหรับการแก้ไขปัญหาเพิ่มเติม โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="e94cd-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="e94cd-117">ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งานและข้อผิดพลาดในการเปิดใช้งานใน Office</span><span class="sxs-lookup"><span data-stu-id="e94cd-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="e94cd-118">"ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณ โปรดลองอีกครั้งในภายหลัง"</span><span class="sxs-lookup"><span data-stu-id="e94cd-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)