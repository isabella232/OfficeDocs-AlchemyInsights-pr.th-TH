---
title: ไม่สามารถเปิดใช้งาน Office ได้
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: ee4618bd288e3e8be75dc969af58f921a14f48b0
ms.sourcegitcommit: bf87d91fa60bd961bc6c887c4a4be7a3c7665b38
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/01/2020
ms.locfileid: "44474516"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="066fa-102">ไม่สามารถเปิดใช้งาน Office ได้</span><span class="sxs-lookup"><span data-stu-id="066fa-102">Unable to activate Office</span></span>

- <span data-ttu-id="066fa-103">ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="066fa-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="066fa-104">ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตให้สิทธิ์การใช้งานไคลเอ็นต์ เช่น Office 365 Business หรือ Business Premium[และให้แน่ใจว่าผู้ใช้มีสิทธิ์การใช้งานที่มอบหมาย](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="066fa-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="066fa-105">ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้ Office ด้วยบัญชีผู้ใช้เดียวกันกับที่มีการกําหนดสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="066fa-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="066fa-106">ตรวจสอบ[หน้าความสมบูรณ์ของบริการ Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health)เพื่อดูว่ามีปัญหาใด ๆ ที่ทราบเกี่ยวกับบริการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="066fa-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="066fa-107">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าไฟร์วอลล์ไม่ได้บล็อกการเข้าถึงแอป Office กับอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="066fa-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Office apps access to the internet.</span></span> <span data-ttu-id="066fa-108">โปรดดู[Url ของ Office 365 และช่วงที่อยู่ IP](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "ช่วง URL และที่อยู่ IP ของ Office 365")</span><span class="sxs-lookup"><span data-stu-id="066fa-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="066fa-109">ใช้การดําเนินการแก้ไขปัญหาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="066fa-109">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="066fa-110">เปิดแอป Office และ[ออกจากระบบ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)บัญชีผู้ใช้ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="066fa-110">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="066fa-111">[เอาออก](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "เอา")และมอบหมายสิทธิ์การใช้งาน Office[ใหม่](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "มอบหมายใหม่")และจากนั้น[เข้าสู่ระบบ Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "ลงชื่อเข้าใช้สํานักงาน")โดยใช้บัญชีผู้ใช้ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="066fa-111">[Remove](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Remove") and [re-assign](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "re-assign") Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "sign into Office") using the affected user account.</span></span>
- <span data-ttu-id="066fa-112">เรียกใช้[ตัวแก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="066fa-112">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="066fa-113">รีเซ็ตสถานะการเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="066fa-113">Reset Office activation state</span></span>](https://docs.microsoft.com/en-us/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "รีเซ็ตสถานะการเปิดใช้งาน Office")
- [<span data-ttu-id="066fa-114">ดําเนินการซ่อมแซมสํานักงานแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="066fa-114">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="066fa-115">สําหรับการแก้ไขปัญหาเพิ่มเติม โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="066fa-115">For additional troubleshooting solutions, see:</span></span>  
[<span data-ttu-id="066fa-116">ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งานและข้อผิดพลาดในการเปิดใช้งานใน Office</span><span class="sxs-lookup"><span data-stu-id="066fa-116">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)  
<span data-ttu-id="066fa-117">["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณ</span><span class="sxs-lookup"><span data-stu-id="066fa-117">["Sorry, we can't connect to your account.</span></span> <span data-ttu-id="066fa-118">โปรดลองอีกครั้งในภายหลัง" https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365</span><span class="sxs-lookup"><span data-stu-id="066fa-118">Please try again later" error when you activate Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 ""Sorry, we can't connect to your account.</span></span> <span data-ttu-id="066fa-119">โปรดลองอีกครั้งในภายหลัง"ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office")</span><span class="sxs-lookup"><span data-stu-id="066fa-119">Please try again later" error when you activate Office")</span></span>