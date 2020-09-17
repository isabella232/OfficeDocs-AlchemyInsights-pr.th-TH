---
title: สร้างและแชร์ปฏิทินของโฟลเดอร์สาธารณะใน Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804082"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="62284-102">สร้างและแชร์ปฏิทินของโฟลเดอร์สาธารณะใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="62284-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="62284-103">คุณสามารถสร้างปฏิทินในโฟลเดอร์สาธารณะได้จากไคลเอ็นต์ Outlook บนเดสก์ท็อปเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="62284-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="62284-104">ใช้ขั้นตอนเหล่านี้เพื่อตั้งค่าปฏิทินของโฟลเดอร์สาธารณะ:</span><span class="sxs-lookup"><span data-stu-id="62284-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="62284-105">ตรวจสอบให้แน่ใจว่ามีการจัดวางโฟลเดอร์สาธารณะใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="62284-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="62284-106">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่สร้างกล่องจดหมายโฟลเดอร์สาธารณะ](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox)</span><span class="sxs-lookup"><span data-stu-id="62284-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="62284-107">ตรวจสอบให้แน่ใจว่าคุณได้กำหนดสิทธิ์การเข้าถึงที่จำเป็นเพื่อสร้างโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="62284-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="62284-108">สำหรับข้อมูลเพิ่มเติมให้ดูที่[สิทธิ์ของโฟลเดอร์สาธารณะสำหรับ Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)</span><span class="sxs-lookup"><span data-stu-id="62284-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="62284-109">ลงชื่อเข้าใช้ไคลเอ็นต์เดสก์ท็อปของ Outlook และตรวจสอบให้แน่ใจว่าคุณสามารถเข้าถึงการปรับใช้โฟลเดอร์สาธารณะของคุณได้</span><span class="sxs-lookup"><span data-stu-id="62284-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="62284-110">ถ้าคุณกำลังมีปัญหาในการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ไคลเอ็นต์เดสก์ท็อปของ Outlook ให้ดูที่[ผู้ใช้ Exchange Online ไม่สามารถเชื่อมต่อกับโฟลเดอร์สาธารณะได้โดยใช้ Outlook หรือ OWA](https://aka.ms/pfcte)</span><span class="sxs-lookup"><span data-stu-id="62284-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="62284-111">สร้างชนิดปฏิทินของโฟลเดอร์สาธารณะใหม่</span><span class="sxs-lookup"><span data-stu-id="62284-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="62284-112">โฟลเดอร์สาธารณะจะถูกแชร์กับผู้ใช้อื่นทั้งหมดตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="62284-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="62284-113">เจ้าของโฟลเดอร์สาธารณะสามารถเปลี่ยนแปลงสิทธิ์จากไคลเอ็นต์เดสก์ท็อปของ Outlook ได้</span><span class="sxs-lookup"><span data-stu-id="62284-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="62284-114">สำหรับข้อมูลเพิ่มเติมให้ดูที่[สิทธิ์ของโฟลเดอร์สาธารณะสำหรับ Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)</span><span class="sxs-lookup"><span data-stu-id="62284-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="62284-115">**หมายเหตุ:** ปฏิทินโฟลเดอร์สาธารณะได้รับการออกแบบมาเพื่อใช้ภายในองค์กรและไม่สามารถเผยแพร่บนอินเทอร์เน็ตได้</span><span class="sxs-lookup"><span data-stu-id="62284-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="62284-116">ใช้กล่องจดหมายที่แชร์ถ้าความตั้งใจของคุณคือการประกาศปฏิทินบนอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="62284-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>