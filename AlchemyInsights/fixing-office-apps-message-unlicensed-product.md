---
title: ไม่สามารถเปิดใช้งานOffice
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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798699"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="2e29a-102">ไม่สามารถเปิดใช้งานOffice</span><span class="sxs-lookup"><span data-stu-id="2e29a-102">Unable to activate Office</span></span>

<span data-ttu-id="2e29a-103">**หมายเหตุ**: ถ้าคุณใช้งานเวอร์ชันที่เก่ากว่าWindows (ตัวอย่างเช่น Windows 7) ตรวจสอบให้แน่ใจว่าเปิดใช้งาน TLS 1.2 เป็นค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="2e29a-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="2e29a-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="2e29a-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="2e29a-105">ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="2e29a-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="2e29a-106">ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตสิทธิ์การใช้งานไคลเอ็นต์ เช่น Office 365 Business หรือ business Premium[และตรวจสอบให้แน่ใจว่าผู้ใช้ได้มอบหมายสิทธิ์การใช้งาน](/microsoft-365/admin/manage/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="2e29a-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="2e29a-107">ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้Officeด้วยบัญชีเดียวกันกับที่ได้รับการมอบหมายสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="2e29a-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="2e29a-108">ตรวจสอบ[Office 365สถานภาพ](/office365/enterprise/view-service-health)บริการเพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="2e29a-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="2e29a-109">ตรวจสอบการตั้งค่าไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และพร็อกซีของคุณเพื่อยืนยันว่าไม่ได้บล็อกMicrosoft 365ไม่ให้เข้าถึงอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="2e29a-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="2e29a-110">โปรดดู[Office 365 URL และช่วงที่อยู่](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL และช่วงที่อยู่ IP")IP</span><span class="sxs-lookup"><span data-stu-id="2e29a-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="2e29a-111">**เคล็ดลับ** บนคอมพิวเตอร์Windows เราจะสามารถวินิจฉัยและแก้ไขปัญหาการOfficeลงชื่อเข้าใช้ทั่วไปต่างๆ ให้คุณโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="2e29a-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="2e29a-112">ดาวน์โหลดและเรียกใช้ **[Microsoft ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SaRA-OfficeSignInScenario)** เพื่อใช้เครื่องมืออัตโนมัติของเรา</span><span class="sxs-lookup"><span data-stu-id="2e29a-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="2e29a-113">ใช้การแอคชันการแก้ไขปัญหาต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="2e29a-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="2e29a-114">เปิดแอป Office[และ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)ลงชื่อออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="2e29a-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="2e29a-115">[เอาออก](/microsoft-365/admin/manage/remove-licenses-from-users)[และ re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and [then sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span><span class="sxs-lookup"><span data-stu-id="2e29a-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="2e29a-116">เรียกใช้ [ตัวแก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="2e29a-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="2e29a-117">ตั้งค่าสถานะOfficeเปิดใช้งานใหม่</span><span class="sxs-lookup"><span data-stu-id="2e29a-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "ตั้งค่าสถานะOfficeเปิดใช้งานใหม่")
- [<span data-ttu-id="2e29a-118">ใช้การซ่อมแซมแบบออนไลน์ของOffice</span><span class="sxs-lookup"><span data-stu-id="2e29a-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="2e29a-119">ดูวิธีแก้ไขปัญหาเพิ่มเติมที่:</span><span class="sxs-lookup"><span data-stu-id="2e29a-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="2e29a-120">ข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาตและการเปิดใช้งานในOffice</span><span class="sxs-lookup"><span data-stu-id="2e29a-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="2e29a-121">"ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง" ข้อผิดพลาดเมื่อคุณOffice</span><span class="sxs-lookup"><span data-stu-id="2e29a-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)