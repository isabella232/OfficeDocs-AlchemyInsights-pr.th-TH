---
title: การแก้ข้อผิดพลาดของผลิตภัณฑ์ที่มีสิทธิ์
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
ms.openlocfilehash: 178811c81775b22676a0106283be4e516d40a95b
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628045"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="b7dea-102">ข้อเสนอแนะสำหรับการแก้ข้อผิดพลาด "ผลิตภัณฑ์ที่ไม่มีสิทธิ์"</span><span class="sxs-lookup"><span data-stu-id="b7dea-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="b7dea-103">หากต้องการแก้ไขข้อผิดพลาดเกี่ยวกับ "ผลิตภัณฑ์ที่มีสิทธิ์" ให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b7dea-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="b7dea-104">ตรวจสอบดูว่าสถานะการสมัครสมาชิกของคุณหมดอายุแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="b7dea-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="b7dea-105">ตรวจสอบให้แน่ใจว่าคุณมีการบอกรับเป็นสมาชิกที่อนุญาตให้ใบอนุญาตของไคลเอ็นต์เช่น Office ๓๖๕ธุรกิจหรือ Business Premium และ[ให้แน่ใจว่าผู้ใช้ที่มีการมอบหมายใบอนุญาต](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="b7dea-105">Make sure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span> 
- <span data-ttu-id="b7dea-106">ตรวจสอบให้แน่ใจว่าผู้ใช้กำลังเข้าสู่ระบบ Office ด้วยบัญชีเดียวกันที่ได้รับมอบหมายใบอนุญาต</span><span class="sxs-lookup"><span data-stu-id="b7dea-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="b7dea-107">ตรวจสอบ[หน้าความสมบูรณ์ของบริการ Office ๓๖๕](https://docs.microsoft.com/office365/enterprise/view-service-health)เพื่อดูว่ามีปัญหาที่ทราบกับบริการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="b7dea-107">Check the [Office 365 Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="b7dea-108">ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกการเข้าถึงแอป Office ไปยังอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="b7dea-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Office apps access to the Internet.</span></span> <span data-ttu-id="b7dea-109">ดู[url ของ Office ๓๖๕และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="b7dea-109">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="b7dea-110">นอกจากนี้คุณอาจลองใช้การแก้ไขปัญหาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b7dea-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="b7dea-111">เปิดแอป Office แล้ว[ลงชื่อออก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)จากบัญชีผู้ใช้ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="b7dea-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="b7dea-112">[เอาออก](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users)และ[มอบ](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users)หมายใบอนุญาต office ใหม่และจากนั้น[เข้าสู่ระบบ Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="b7dea-112">[Remove](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="b7dea-113">เรียกใช้ตัว[แก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="b7dea-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="b7dea-114">[รีเซ็ตสถานะการเปิดใช้งาน Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="b7dea-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="b7dea-115">[ดำเนินการซ่อมแซมทางออนไลน์ของสำนักงาน](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="b7dea-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="b7dea-116">สำหรับโซลูชันการแก้ไขปัญหาเพิ่มเติมโปรดดูที่:</span><span class="sxs-lookup"><span data-stu-id="b7dea-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="b7dea-117">ข้อผิดพลาดของผลิตภัณฑ์และการเปิดใช้งานใน Office</span><span class="sxs-lookup"><span data-stu-id="b7dea-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="b7dea-118">"ขออภัยเราไม่สามารถเชื่อมต่อกับบัญชีของคุณ กรุณาลองอีกครั้งในภายหลัง "ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="b7dea-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)