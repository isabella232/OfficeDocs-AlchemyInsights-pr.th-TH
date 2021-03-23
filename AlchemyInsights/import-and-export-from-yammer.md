---
title: นําเข้าและส่งออกจาก Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037256"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="2cf57-102">นําเข้าและส่งออกจาก Yammer</span><span class="sxs-lookup"><span data-stu-id="2cf57-102">Import and export from Yammer</span></span>

<span data-ttu-id="2cf57-103">**นําเข้า**</span><span class="sxs-lookup"><span data-stu-id="2cf57-103">**Import**</span></span>

<span data-ttu-id="2cf57-104">ตัวเลือกการนําเข้าของผู้ใช้จะแตกต่างกันโดยขึ้นอยู่กับว่าเครือข่าย Yammer ของคุณ [อยู่ในโหมดดั้งเดิมของ Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)หรือไม่</span><span class="sxs-lookup"><span data-stu-id="2cf57-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="2cf57-105">**โหมดที่ไม่ใช่โหมด** ดั้งเดิม: ผู้ใช้สามารถนําเข้าไปยังกลุ่มโดยใช้ [เพิ่ม](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) จากสมุดรายชื่อ (จํากัดให้ผู้ใช้ 100 ราย) ภายในการตั้งค่ากลุ่ม หรือเครือข่ายโดยใช้ อัปเดตเป็นกลุ่ม [ภายในผู้ดูแลระบบ](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="2cf57-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="2cf57-106">**โหมดดั้งเดิม**: การเป็นสมาชิกกลุ่มและการดําเนินการเป็นสมาชิกเครือข่ายควรดําเนินการจากพอร์ทัลผู้ดูแลระบบ [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)พอร์ทัล [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)หรือใช้ตัวเลือก Azure AD อื่น</span><span class="sxs-lookup"><span data-stu-id="2cf57-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="2cf57-107">เครือข่ายในโหมดดั้งเดิมจะไม่มีสิทธิ์เข้าถึงการอัปเดตเป็นกลุ่มและฟีเจอร์ดั้งเดิมอื่นๆ อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="2cf57-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2cf57-108">Yammer ไม่สนับสนุนการนําเข้าเนื้อหาจากภายในผู้ดูแลระบบเครือข่าย แม้ว่าจะมีการใช้งานฟีเจอร์การส่งออกข้อมูลในเครือข่ายอื่น</span><span class="sxs-lookup"><span data-stu-id="2cf57-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="2cf57-109">เนื้อหาสามารถโพสต์ใหม่ได้โดยโซลูชันของคู่ค้าหรือ API ของ Yammer REST</span><span class="sxs-lookup"><span data-stu-id="2cf57-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="2cf57-110">**ส่งออก**</span><span class="sxs-lookup"><span data-stu-id="2cf57-110">**Export**</span></span>

<span data-ttu-id="2cf57-111">[ส่งออกข้อมูลเครือข่ายภายในผู้ดูแลระบบ](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) เครือข่ายอนุญาตให้ส่งออกเนื้อหาจากเครือข่าย Yammer รวมถึงข้อความและไฟล์</span><span class="sxs-lookup"><span data-stu-id="2cf57-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="2cf57-112">สิ่งที่แนบมาอาจมีขนาดใหญ่มาก และจะทําให้การส่งออกใช้เวลานานในการทําให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="2cf57-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="2cf57-113">เราขอแนะให้เครือข่ายที่ใช้งานอยู่ถูกส่งออกโดยใช้ [API การส่งออก](https://developer.yammer.com/docs/data-export-api) ข้อมูลในช่วงตามวันหรือสัปดาห์</span><span class="sxs-lookup"><span data-stu-id="2cf57-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="2cf57-114">ฝ่ายสนับสนุนของ Microsoft ไม่มีสคริปต์แบบปรับแต่งเองเพื่อวัตถุประสงค์นี้</span><span class="sxs-lookup"><span data-stu-id="2cf57-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="2cf57-115">มี [การส่งออก GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) แยกต่างหากเพื่อส่งออกเนื้อหาให้กับผู้ใช้แต่ละราย</span><span class="sxs-lookup"><span data-stu-id="2cf57-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>