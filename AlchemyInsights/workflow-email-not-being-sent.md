---
title: ไม่มีการส่งอีเมลของเวิร์กโฟลว์
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749028"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="6e7e1-102">ไม่มีการส่งอีเมลของเวิร์กโฟลว์สำหรับรายการหรือไลบรารี SharePoint</span><span class="sxs-lookup"><span data-stu-id="6e7e1-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="6e7e1-103">อีเมลจากเวิร์กโฟลว์จะไม่ถูกส่งไปยังผู้ใช้ทั้งหมดหรือเฉพาะผู้ใช้ที่ระบุเท่านั้นหรือคุณเห็นข้อผิดพลาด**ที่ไม่สามารถส่งข้อความอีเมลได้ตรวจสอบให้แน่ใจว่าอีเมลมีผู้รับที่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="6e7e1-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="6e7e1-104">ตรวจสอบว่าผู้ใช้มีอยู่ในกลุ่มสิทธิ์ของ **บุคคลทั้งหมด** (รายการข้อมูลผู้ใช้) สำหรับไซต์คอลเลกชันนั้นหรือไม่</span><span class="sxs-lookup"><span data-stu-id="6e7e1-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="6e7e1-105">ตัวอย่าง URL โดยตรง: https:// <tenant> sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="6e7e1-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="6e7e1-106">ถ้าไม่มีผู้ใช้ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้หน้า</span><span class="sxs-lookup"><span data-stu-id="6e7e1-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="6e7e1-107">ถ้าเป็นผู้ใช้ภายนอกตรวจสอบให้แน่ใจว่าการเชิญของพวกเขาได้รับการยอมรับแล้ว</span><span class="sxs-lookup"><span data-stu-id="6e7e1-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="6e7e1-108">ถ้าผู้ใช้มีอยู่ในกลุ่มสิทธิ์ตรวจสอบให้แน่ใจว่าที่อยู่อีเมลนั้นถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="6e7e1-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="6e7e1-109">ถ้าที่อยู่อีเมลของผู้ใช้ไม่ได้ตั้งค่าที่นี่จากนั้นสร้างการแจ้งเตือนตัวอย่างสำหรับผู้ใช้ที่บังคับให้มีการซิงค์บัญชีผู้ใช้นั้นจากโปรไฟล์ผู้ใช้ของ SharePoint ไปยังไซต์คอลเลกชันนี้</span><span class="sxs-lookup"><span data-stu-id="6e7e1-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="6e7e1-110">อีเมลจากเวิร์กโฟลว์จะถูกส่งไปยังผู้ดูแลไซต์คอลเลกชันแต่ไม่ใช่ผู้ใช้อื่นและดูข้อผิดพลาด**HTTP ที่ห้ามใช้<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**</span><span class="sxs-lookup"><span data-stu-id="6e7e1-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="6e7e1-111">ให้ดูที่[การเข้าถึงถูกปฏิเสธเมื่อคุณส่งอีเมลไปยังกลุ่ม SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)</span><span class="sxs-lookup"><span data-stu-id="6e7e1-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="6e7e1-112">นอกจากนี้ให้ตรวจสอบว่าฟีเจอร์ไซต์คอลเลกชัน **สิทธิ์ของผู้ใช้ที่มีสิทธิ์การเข้าถึงแบบจำกัด** ไม่ได้ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="6e7e1-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="6e7e1-113">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="6e7e1-113">Related topics</span></span>
<span data-ttu-id="6e7e1-114">ต้องการลองใช้ Microsoft Flow ใน SharePoint Online หรือไม่</span><span class="sxs-lookup"><span data-stu-id="6e7e1-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="6e7e1-115">สร้างขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="6e7e1-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6e7e1-116">SharePoint และการไหล</span><span class="sxs-lookup"><span data-stu-id="6e7e1-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


