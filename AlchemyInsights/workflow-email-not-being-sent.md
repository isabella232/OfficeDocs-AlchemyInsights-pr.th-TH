---
title: ไม่มีการส่งอีเมลลําดับงาน
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766152"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="3f5e0-102">ไม่มีการส่งอีเมลลําดับงานสําหรับรายการหรือไลบรารี SharePoint</span><span class="sxs-lookup"><span data-stu-id="3f5e0-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="3f5e0-103">อีเมลจากเวิร์กโฟลว์จะไม่ถูกส่งไปยังผู้ใช้ทั้งหมดหรือเฉพาะผู้ใช้ที่ระบุ หรือ**คุณเห็นข้อผิดพลาด ตรวจสอบให้แน่ใจว่าอีเมลมีผู้รับที่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="3f5e0-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="3f5e0-104">ตรวจสอบว่าผู้ใช้ที่มีอยู่ในกลุ่มสิทธิ์**บุคคลทั้งหมด**(รายการข้อมูลผู้ใช้) สําหรับไซต์คอลเลกชันนั้นหรือไม่</span><span class="sxs-lookup"><span data-stu-id="3f5e0-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="3f5e0-105">ตัวอย่าง URL โดยตรง<tenant>:<sitename>https:// .sharepoint.com/sites/ / _layouts / 15 / people.aspx? สมาชิกกลุ่มId = 0</span><span class="sxs-lookup"><span data-stu-id="3f5e0-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="3f5e0-106">ถ้าผู้ใช้ไม่มี อยู่ ตรวจสอบให้แน่ใจว่า ผู้ใช้ได้ลงชื่อเข้าใช้ในเพจ</span><span class="sxs-lookup"><span data-stu-id="3f5e0-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="3f5e0-107">ถ้าเป็นผู้ใช้ภายนอก ให้ตรวจสอบว่าคําเชิญของพวกเขาได้รับการยอมรับแล้ว</span><span class="sxs-lookup"><span data-stu-id="3f5e0-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="3f5e0-108">ถ้าผู้ใช้ไม่มีอยู่ในกลุ่มสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="3f5e0-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="3f5e0-109">ถ้าไม่ได้ตั้งค่าที่อยู่อีเมลของผู้ใช้ที่นี่ แล้วสร้างการแจ้งเตือนตัวอย่างสําหรับผู้ใช้ที่บังคับให้ซิงค์ของบัญชีผู้ใช้นั้นจากโปรไฟล์ผู้ใช้ของ SharePoint ไปยังไซต์คอลเลกชันนี้</span><span class="sxs-lookup"><span data-stu-id="3f5e0-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="3f5e0-110">อีเมลจากเวิร์กโฟลว์จะถูกส่งไปยังผู้ดูแลไซต์คอลเลกชัน แต่ไม่ให้ผู้ใช้อื่น เห็นข้อผิดพลาด HTTP Forbidden เป็น**<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.SendEmail**</span><span class="sxs-lookup"><span data-stu-id="3f5e0-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="3f5e0-111">ดู[การเข้าถึงถูกปฏิเสธเมื่อคุณส่งอีเมลไปยังกลุ่ม SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)</span><span class="sxs-lookup"><span data-stu-id="3f5e0-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="3f5e0-112">นอกจากนี้ ตรวจสอบว่า ผู้ใช้สิทธิ์**lockdown**จํากัดสิทธิ์ผู้ใช้คุณลักษณะชุดเก็บรวบรวมไซต์</span><span class="sxs-lookup"><span data-stu-id="3f5e0-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="3f5e0-113">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="3f5e0-113">Related topics</span></span>
<span data-ttu-id="3f5e0-114">ต้องการลอง Microsoft ไหลใน SharePoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="3f5e0-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="3f5e0-115">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="3f5e0-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="3f5e0-116">SharePoint และโฟลว์</span><span class="sxs-lookup"><span data-stu-id="3f5e0-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


