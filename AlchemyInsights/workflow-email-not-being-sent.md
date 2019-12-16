---
title: ไม่มีการส่ง email ของลำดับงาน
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049392"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="170b4-102">ไม่มีการส่งเมลของลำดับงานสำหรับรายการหรือไลบรารี SharePoint</span><span class="sxs-lookup"><span data-stu-id="170b4-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="170b4-103">ไม่มีส่งจดหมายจากเวิร์กโฟลว์ไปยังผู้ใช้ทั้งหมดหรือเฉพาะผู้ใช้หรือคุณเห็นข้อผิดพลาด**ที่ไม่สามารถส่งข้อความทาง e-mail ตรวจสอบให้แน่ใจว่า e-mail มีผู้รับที่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="170b4-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="170b4-104">ตรวจสอบว่าผู้ใช้มีอยู่ในกลุ่มสิทธิ์**คนทั้งหมด**(รายการข้อมูลผู้ใช้) สำหรับไซต์คอลเลกชันนั้น</span><span class="sxs-lookup"><span data-stu-id="170b4-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="170b4-105">ตัวอย่าง URL โดยตรง<tenant>: https://<sitename>/_layouts/15/sharepoint.com/sites/? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="170b4-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="170b4-106">ถ้าผู้ใช้ไม่มีอยู่โปรดตรวจสอบให้แน่ใจว่าผู้ใช้ที่มีการลงชื่อเข้าสู่หน้าเว็บ</span><span class="sxs-lookup"><span data-stu-id="170b4-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="170b4-107">หากเป็นผู้ใช้ภายนอกโปรดตรวจสอบให้แน่ใจว่าได้ยอมรับคำเชิญของพวกเขาแล้ว</span><span class="sxs-lookup"><span data-stu-id="170b4-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="170b4-108">ถ้าผู้ใช้ไม่มีอยู่ในกลุ่มสิทธิ์โปรดตรวจสอบให้แน่ใจว่าที่อยู่ของเมลไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="170b4-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="170b4-109">ถ้าไม่ได้ตั้งค่าที่อยู่ e-mail ของผู้ใช้ที่นี่แล้วสร้างการแจ้งเตือนตัวอย่างสำหรับผู้ใช้ที่บังคับให้ซิงค์ของบัญชีผู้ใช้นั้นจากโปรไฟล์ผู้ใช้ของ SharePoint ไปยังไซต์คอลเลกชันนี้</span><span class="sxs-lookup"><span data-stu-id="170b4-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="170b4-110">มีส่งจดหมายจากเวิร์กโฟลว์ไปยังผู้ดูแลชุดเก็บรวบรวมไซต์แต่ไม่ได้ให้กับคนอื่นและดูข้อผิดพลาด**HTTP ต้องห้ามไปยัง<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**</span><span class="sxs-lookup"><span data-stu-id="170b4-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="170b4-111">ดูการ[เข้าถึงถูกปฏิเสธเมื่อคุณส่งเมลไปยังกลุ่ม SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)</span><span class="sxs-lookup"><span data-stu-id="170b4-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="170b4-112">นอกจากนี้ให้ตรวจสอบว่าการ**เข้าถึงแบบจำกัดสิทธิ์ผู้ใช้โหมด lockdown**ไซต์คอลเลกชันไม่ทำงาน</span><span class="sxs-lookup"><span data-stu-id="170b4-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="170b4-113">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="170b4-113">Related topics</span></span>
<span data-ttu-id="170b4-114">ต้องการลองการไหลของ Microsoft ใน SharePoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="170b4-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="170b4-115">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="170b4-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="170b4-116">SharePoint และการไหล</span><span class="sxs-lookup"><span data-stu-id="170b4-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


