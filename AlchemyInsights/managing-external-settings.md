---
title: การจัดการการตั้งค่าภายนอก
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294431"
---
# <a name="managing-external-settings"></a><span data-ttu-id="60bb5-102">การจัดการการตั้งค่าภายนอก</span><span class="sxs-lookup"><span data-stu-id="60bb5-102">Managing External Settings</span></span>

<span data-ttu-id="60bb5-103">**การประกาศ**</span><span class="sxs-lookup"><span data-stu-id="60bb5-103">**Announcement**</span></span>

- <span data-ttu-id="60bb5-104">[การเลิกใช้การสนับสนุนการลงชื่อเข้าใช้ WebView จาก Google ตั้งแต่วันที่ 4 มกราคม 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="60bb5-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="60bb5-105">ทดสอบว่าแอปของคุณได้รับผลกระทบจากตามแนวทางของ Google เกี่ยวกับการทดสอบความเข้ากันได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="60bb5-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="60bb5-106">ตรวจสอบให้แน่ใจว่าได้ใช้มุมมองเว็บของระบบหรือเบราว์เซอร์ระบบเมื่อลงชื่อเข้าใช้ผู้ใช้ของคุณด้วยบัญชี Google ของผู้ใช้ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="60bb5-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="60bb5-107">**จัดการการตั้งค่าการเชิญ**</span><span class="sxs-lookup"><span data-stu-id="60bb5-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="60bb5-108">ยืนยันว่าคุณได้กําหนด [ค่าการตั้งค่าการร่วมมือกัน](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) ภายนอกเพื่อให้บุคคลที่เหมาะสมสามารถส่งคําเชิญได้</span><span class="sxs-lookup"><span data-stu-id="60bb5-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="60bb5-109">**จัดการสิทธิ์การเข้าถึงของผู้ใช้ที่เป็นแขก**</span><span class="sxs-lookup"><span data-stu-id="60bb5-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="60bb5-110">ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์การเข้าถึงของแขกในไดเรกทอรีผ่านพอร์ทัล Azure โดยการกําหนดค่าสิทธิ์การเข้าถึงของผู้ใช้ภายนอกบนหน้าการตั้งค่าการร่วมมือกันภายนอก</span><span class="sxs-lookup"><span data-stu-id="60bb5-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="60bb5-111">[เรียนรู้เพิ่มเติมเกี่ยวกับการตั้งค่า](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)นี้</span><span class="sxs-lookup"><span data-stu-id="60bb5-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="60bb5-112">หากคุณต้องการให้แขกของคุณเข้าถึงแอป เช่น Teams หรือ SharePoint ให้ยืนยันว่าคุณได้กําหนดค่าแอปเหล่านั้นให้อนุญาตการเข้าถึงของแขกแล้ว</span><span class="sxs-lookup"><span data-stu-id="60bb5-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="60bb5-113">เรียนรู้เพิ่มเติมเกี่ยวกับการตั้งค่า[Teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [และ SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="60bb5-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="60bb5-114">**การกําหนดค่าคําเชิญ:**</span><span class="sxs-lookup"><span data-stu-id="60bb5-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="60bb5-115">เปิดใช้งานการร่วมมือกันภายนอก B2B และจัดการผู้ที่สามารถเชิญผู้ใช้ภายนอกได้</span><span class="sxs-lookup"><span data-stu-id="60bb5-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="60bb5-116">อนุญาตหรือบล็อกคําเชิญให้ผู้ใช้จากองค์กรที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="60bb5-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="60bb5-117">**การกําหนดค่าผู้ให้บริการข้อมูลเฉพาะตัวที่อนุญาต:**</span><span class="sxs-lookup"><span data-stu-id="60bb5-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="60bb5-118">การติดต่อกับภายนอกของ Google</span><span class="sxs-lookup"><span data-stu-id="60bb5-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="60bb5-119">การติดต่อกับภายนอกโดยตรง</span><span class="sxs-lookup"><span data-stu-id="60bb5-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="60bb5-120">ส่งอีเมลการรับรองความถูกต้องรหัสผ่านแบบใช้เวลาเดียว</span><span class="sxs-lookup"><span data-stu-id="60bb5-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
