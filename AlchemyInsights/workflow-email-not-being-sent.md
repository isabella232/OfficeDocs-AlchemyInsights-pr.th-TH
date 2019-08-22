---
title: ไม่มีการส่งอีเมลการเวิร์กโฟลว์
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530910"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="44967-102">ไม่มีการส่งอีเมลลำดับงานสำหรับรายการ SharePoint หรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="44967-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="44967-103">อีเมลจากเวิร์กโฟลว์จะไม่ถูกส่งถึงผู้ใช้ทั้งหมดหรือผู้ใช้ที่ระบุเท่านั้น หรือคุณเห็นข้อความอีเม**ข้อผิดพลาดไม่สามารถส่ง ตรวจสอบว่า อีเมลที่มีผู้รับที่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="44967-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="44967-104">ตรวจสอบว่ามีผู้ใช้ในกลุ่มสิทธิ์**ทุกคน**(รายการข้อมูลผู้ใช้) สำหรับไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="44967-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="44967-105">ตัวอย่าง URL โดยตรง: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx หรือไม่ MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="44967-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="44967-106">ถ้าผู้ใช้ไม่มีอยู่ ทำให้แน่ใจว่า ผู้ใช้มีการเซ็นชื่อลงในเพจ</span><span class="sxs-lookup"><span data-stu-id="44967-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="44967-107">ถ้าคุณเป็นผู้ใช้ภายนอก โปรดตรวจสอบให้แน่ใจว่า มีการยอมรับการเชิญ</span><span class="sxs-lookup"><span data-stu-id="44967-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="44967-108">ถ้ามีผู้ใช้ในกลุ่มสิทธิ์ ทำให้แน่ใจว่า อยู่อีเมลที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="44967-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="44967-109">ถ้าอยู่อีเมลของผู้ใช้ถูกกำหนดที่นี่ สร้างตัวอย่างข้อความแจ้งเตือนสำหรับผู้ใช้ซึ่งเป็นบังคับการซิงค์ของบัญชีผู้ใช้นั้นจากโพรไฟล์ผู้ใช้ของ SharePoint เพื่อเก็บรวบรวมไซต์นี้</span><span class="sxs-lookup"><span data-stu-id="44967-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="44967-110">อีเมลจากเวิร์กโฟลว์จะถูกส่ง ไปที่ผู้ดูแลชุดเก็บรวบรวมไซต์ แต่ไม่ใช่ กับผู้ใช้รายอื่น และดูข้อผิดพลาด**อนุญาตให้ใช้ HTTP <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**</span><span class="sxs-lookup"><span data-stu-id="44967-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="44967-111">ดูการ[เข้าถึงถูกปฏิเสธเมื่อคุณส่งอีเมลให้กับกลุ่ม SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)</span><span class="sxs-lookup"><span data-stu-id="44967-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="44967-112">ตรวจสอบด้วย ว่า คุณลักษณะ**โหมด lockdown สิทธิ์ของผู้ใช้ถูกจำกัดการเข้าถึง**ไซต์คอลเลกชันไม่ได้ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="44967-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="44967-113">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="44967-113">Related topics</span></span>
<span data-ttu-id="44967-114">ต้องการลองกระแส Microsoft ใน SharePoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="44967-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="44967-115">สร้างขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="44967-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="44967-116">SharePoint และขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="44967-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


