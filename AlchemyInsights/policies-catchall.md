---
title: นโยบาย catchall
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "3207"
ms.openlocfilehash: e5d08462e8662fa1651ad81235d0efd5fc4bac58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721313"
---
# <a name="teams-policies"></a><span data-ttu-id="aba87-102">นโยบายของทีม</span><span class="sxs-lookup"><span data-stu-id="aba87-102">Teams policies</span></span>

<span data-ttu-id="aba87-103">การตั้งค่าทีม Microsoft จะถูกควบคุมโดยนโยบาย</span><span class="sxs-lookup"><span data-stu-id="aba87-103">Microsoft Teams settings are controlled by policies.</span></span> <span data-ttu-id="aba87-104">เมื่อต้องการทำการเปลี่ยนแปลงคุณจะต้องกำหนดค่านโยบายที่เหมาะสมแล้วนำไปใช้กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="aba87-104">To make a change, you must configure the appropriate policy, and then apply it to users.</span></span> <span data-ttu-id="aba87-105">วิธีที่รวดเร็วที่สุดในการทำเช่นนี้สำหรับผู้ใช้ทั้งหมดของคุณคือการปรับเปลี่ยนนโยบายเริ่มต้นที่ชื่อว่าส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="aba87-105">The quickest way to do this for all your users is to modify the default policy named Global.</span></span> 

<span data-ttu-id="aba87-106">**หมายเหตุ:** การเปลี่ยนแปลงนโยบายใช้***เวลาอย่างน้อย4จนถึง๔๘ชั่วโมงที่มีผลบังคับใช้***</span><span class="sxs-lookup"><span data-stu-id="aba87-106">**NOTE** Policy changes take ***at least 4 up to 48 hours to take effect***.</span></span> <span data-ttu-id="aba87-107">ถ้าคุณสร้างนโยบายแบบกำหนดเองคุณจำเป็นต้องรออย่างน้อย4ชั่วโมงก่อนที่คุณจะสามารถทำการเปลี่ยนแปลงเพิ่มเติมได้</span><span class="sxs-lookup"><span data-stu-id="aba87-107">If you create a custom policy, you need to wait at least 4 hours before you can make additional changes to it.</span></span> <span data-ttu-id="aba87-108">จากนั้นคุณสามารถนำนโยบายนั้นไปใช้กับผู้ใช้ได้</span><span class="sxs-lookup"><span data-stu-id="aba87-108">Then you can apply that policy to users.</span></span> <span data-ttu-id="aba87-109">ซึ่งหมายความว่านโยบายแบบกำหนดเองอาจใช้เวลาถึง๔๘ชั่วโมงจึงจะมีผลใช้ได้</span><span class="sxs-lookup"><span data-stu-id="aba87-109">This means that custom policies can take up to 48 hours to take effect.</span></span> <span data-ttu-id="aba87-110">นโยบายส่วนกลางจะถูกตั้งค่าเป็นค่าเริ่มต้นสำหรับผู้ใช้ทั้งหมดและการเปลี่ยนแปลงที่เกิดขึ้นกับนโยบายส่วนกลางอาจใช้เวลาถึง24ชั่วโมงเพื่อให้มีผลใช้งาน</span><span class="sxs-lookup"><span data-stu-id="aba87-110">Global policies are set as default for all users, and changes to the Global policy can take up to 24 hours to take effect.</span></span> <span data-ttu-id="aba87-111">ถ้าคุณได้สร้างนโยบายแบบกำหนดเองให้นำไปใช้กับผู้ใช้แล้วและยังไม่ได้นำเอฟเฟ็กต์หลังจาก๔๘ชั่วโมงหรือคุณได้ปรับเปลี่ยนนโยบายส่วนกลางและรออย่างน้อย24ชั่วโมงโปรดเปิดกรณีการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="aba87-111">If you have created a custom policy, applied it to users, and it still hasn't taken effect after 48 hours, or you've modified the Global policy and waited at least 24 hours, please open a support case.</span></span>

<span data-ttu-id="aba87-112">นโยบายของทีมจะแบ่งออกเป็นพื้นที่ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="aba87-112">Teams policies are divided into the following areas:</span></span>

- <span data-ttu-id="aba87-113">[นโยบายของทีม](https://docs.microsoft.com/MicrosoftTeams/teams-policies) ควบคุมการค้นหาของทีมส่วนตัวในการค้นหาและการสร้างช่องทางส่วนตัว</span><span class="sxs-lookup"><span data-stu-id="aba87-113">[Teams policies](https://docs.microsoft.com/MicrosoftTeams/teams-policies) control user discovery of private teams in search and creation of private channels.</span></span>  
- <span data-ttu-id="aba87-114">[นโยบายการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) ควบคุมสิ่งที่ผู้ใช้สามารถทำได้กับการประชุมทีมรวมถึงการควบคุมล็อบบี้</span><span class="sxs-lookup"><span data-stu-id="aba87-114">[Meeting policies](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) control what users can do with Teams meetings, including controlling the lobby.</span></span> <span data-ttu-id="aba87-115">สำหรับความช่วยเหลือเกี่ยวกับปัญหาของล๊อบบี้เช่นการกำหนดค่าทีมให้ยอมรับทุกคนให้ดูที่[การตั้งค่าการควบคุมการตั้งค่าล็อบบี้และระดับการเข้าร่วม](https://docs.microsoft.com/alchemyinsights/bypass-lobby)</span><span class="sxs-lookup"><span data-stu-id="aba87-115">For help with lobby issues, like configuring Teams to admit everyone, see [Control lobby settings and levels of participation](https://docs.microsoft.com/alchemyinsights/bypass-lobby).</span></span>
- <span data-ttu-id="aba87-116">[นโยบายการส่งข้อ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) ความควบคุมสิ่งที่ผู้ใช้สามารถทำได้กับการแชทและข้อความรวมถึงการเปิดหรือปิดการแชท, การลบการแชทร้องขอใบตอบรับการอ่านโดยใช้ giphys และสติกเกอร์และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="aba87-116">[Messaging policies](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) control what users can do with chat and messages, including turning chat on or off, deleting chats, requesting read receipts, using giphys and stickers, and more.</span></span>
- <span data-ttu-id="aba87-117">[นโยบายการตั้งค่าแอปจะ](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) ควบคุมว่าจะให้แอปใดพร้อมใช้งานสำหรับผู้ใช้รวมถึงแอปที่กำหนดเองและแอปของบริษัทอื่นและลำดับที่ปรากฏ</span><span class="sxs-lookup"><span data-stu-id="aba87-117">[App setup policies](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) control which apps are available to users, including custom and third-party apps, and the order in which they appear.</span></span>  
- <span data-ttu-id="aba87-118">[นโยบายการเก็บ](https://docs.microsoft.com/microsoftteams/retention-policies)ข้อมูลของข้อมูลสำหรับทีมจะพบในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายของ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="aba87-118">Data [retention policies](https://docs.microsoft.com/microsoftteams/retention-policies) for Teams are found in the Microsoft 365 security and Compliance Center.</span></span>
- <span data-ttu-id="aba87-119">นโยบายสมุดรายชื่อของทีมจะถูกตั้งค่าผ่านทางการ[ค้นหาไดเรกทอรีลักษณะ](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search)</span><span class="sxs-lookup"><span data-stu-id="aba87-119">Teams address book policies are set via [scoped directory search](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search).</span></span>