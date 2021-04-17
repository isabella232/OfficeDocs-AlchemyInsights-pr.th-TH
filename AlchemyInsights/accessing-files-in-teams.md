---
title: การเข้าถึงไฟล์ใน Teams
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
- "2675"
- "9000710"
ms.openlocfilehash: c6766c318f0058e66950dbd0ca2953b149579a5c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823374"
---
# <a name="accessing-files-in-microsoft-teams"></a><span data-ttu-id="17044-102">การเข้าถึงไฟล์ใน Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="17044-102">Accessing files in Microsoft Teams</span></span>

<span data-ttu-id="17044-103">ถ้าผู้ใช้มีปัญหาในการเข้าถึงไฟล์ใน Microsoft Teams ก่อนอื่นให้พิจารณาว่าไฟล์แนบมากับการสนทนาส่วนตัวหรือการสนทนาในแชนเนล</span><span class="sxs-lookup"><span data-stu-id="17044-103">If users have difficulty accessing a file in Microsoft Teams, first determine whether the file is attached to a private chat or a channel conversation.</span></span> <span data-ttu-id="17044-104">แชนเนลทีมคือที่ที่ทุกคนในทีมสามารถสนทนากันอย่างเปิดกว้าง</span><span class="sxs-lookup"><span data-stu-id="17044-104">Team channels are places where everyone on the team can openly have conversations.</span></span> <span data-ttu-id="17044-105">การแชทส่วนตัวจะมองเห็นได้เฉพาะบุคคลในการแชท (และไฟล์ที่คุณแชร์ในการแชทจะถูกเก็บไว้ใน OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="17044-105">Private chats are only visible to those people in the chat (and files that you share in a chat are stored in OneDrive for Business).</span></span>

<span data-ttu-id="17044-106">เมื่อผู้ใช้แชร์ไฟล์ในการแชทส่วนตัว ไฟล์จะถูกเก็บไว้ใน OneDrive for Business ของผู้ใช้ที่แชร์</span><span class="sxs-lookup"><span data-stu-id="17044-106">When users share files in private chats, the file is stored on the sharing user's OneDrive for Business.</span></span> <span data-ttu-id="17044-107">ถ้าผู้ใช้ถูกเพิ่มลงในการสนทนาส่วนตัวที่มีอยู่ พวกเขาจะไม่สามารถเข้าถึงไฟล์ได้ เว้นแต่เจ้าของเดิมจะแชร์ไฟล์อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="17044-107">If a user was added to an existing private chat, they won't be able to access the files unless the original owner re-shares the file.</span></span>    

<span data-ttu-id="17044-108">**ในการสนทนาในแชนเนล:**</span><span class="sxs-lookup"><span data-stu-id="17044-108">**For channel conversations:**</span></span>

- <span data-ttu-id="17044-109">[การแชร์ไฟล์ใน Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) จะยึดตามการตั้งค่าที่กําหนดค่าใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="17044-109">[Sharing files in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) is based on the settings configured in SharePoint or OneDrive.</span></span> 
- <span data-ttu-id="17044-110">ตรวจสอบ [การร่วมมือกันบนไฟล์กับ](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) ทีม ของคุณ เพื่อเรียนรู้เพิ่มเติมเกี่ยวกับวิธีที่ Teams ช่วยให้องค์กรของคุณสามารถแชร์และร่วมมือกันบนไฟล์ได้</span><span class="sxs-lookup"><span data-stu-id="17044-110">Review [Collaborate on files with your Team](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) to learn more about how Teams allows your organization to share and collaborate on files.</span></span> 
- <span data-ttu-id="17044-111">หากสมาชิกในทีมใหม่พบความล่าช้าในการเข้าถึงไฟล์ โปรดรออย่างน้อย **4** ชั่วโมงก่อนที่จะเปิดตั๋วการสนับสนุนเพื่อให้การลองแบบเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="17044-111">If new team members experience a delay in accessing files, please wait at least **4 hours** before opening a support ticket to allow replication to complete.</span></span> 

<span data-ttu-id="17044-112">If users could previously access files via the Files tab on a team channel, and you get a "these files are no longer available" error, check to see if the SharePoint site or document library has been renamed.</span><span class="sxs-lookup"><span data-stu-id="17044-112">If users could previously access files via the Files tab on a team channel, and you get a "these files are no longer available" error, check to see if the SharePoint site or document library has been renamed.</span></span> <span data-ttu-id="17044-113">การเปลี่ยนชื่อไซต์ SharePoint และไลบรารีเอกสารของ Teams ยังไม่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="17044-113">Renaming SharePoint sites and document libraries for Teams is not yet supported.</span></span> <span data-ttu-id="17044-114">เมื่อต้องการแก้ไขปัญหานี้ ให้เปิดไซต์ทีมที่ใช้กับทีมนี้ แล้วเปลี่ยนชื่อไลบรารีกลับไปเป็น "เอกสารที่แชร์"</span><span class="sxs-lookup"><span data-stu-id="17044-114">To resolve this issue, open the team site used for this team and rename the library back to “Shared Documents”.</span></span>