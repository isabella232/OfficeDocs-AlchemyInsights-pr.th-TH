---
title: การเปลี่ยนแปลงสิทธิ์ของโฟลเดอร์สาธารณะ
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: 68aefd820c681a9022828f67655e1c843692a30e
ms.sourcegitcommit: 92e9a649532f5231ceedcafc4d14b8ad18d517c2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/31/2020
ms.locfileid: "43059791"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="0b8b4-102">การเปลี่ยนแปลงสิทธิ์ของโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="0b8b4-102">Changing public folder permissions</span></span>

<span data-ttu-id="0b8b4-103">สิทธิ์ของโฟลเดอร์สาธารณะสามารถเปลี่ยนแปลงได้โดยผู้ใช้และผู้ดูแลระบบใน Outlook</span><span class="sxs-lookup"><span data-stu-id="0b8b4-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="0b8b4-104">ผู้ดูแลระบบยังสามารถควบคุมสิทธิ์จากศูนย์ดูแล Exchange (EAC), โดยการทําต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0b8b4-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="0b8b4-105">ใน ศูนย์การจัดการ Microsoft 365 ไปที่**ศูนย์การจัดการ**\> **Exchange**</span><span class="sxs-lookup"><span data-stu-id="0b8b4-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="0b8b4-106">เลือก**โฟลเดอร์สาธารณะ**</span><span class="sxs-lookup"><span data-stu-id="0b8b4-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="0b8b4-107">จากที่นั่น คุณสามารถเปลี่ยนสิทธิ์สําหรับโฟลเดอร์สาธารณะแต่ละโฟลเดอร์ได้โดยการกําหนดกลุ่มความปลอดภัยให้กับสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="0b8b4-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="0b8b4-108">สําหรับผู้ใช้เพื่อเปลี่ยนสิทธิ์ของโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="0b8b4-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="0b8b4-109">โปรดทําตามขั้นตอนที่อธิบายไว้ใน[วิธีการวินิจฉัย และแก้ไขปัญหาสิทธิ์ของโฟลเดอร์สาธารณะ](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues)เพื่อแก้ไขปัญหาสิทธิ์ของโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="0b8b4-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="0b8b4-110">**หมายเหตุ**: มีปัญหาที่ทราบอยู่หลายปัญหาที่คุณอาจพบเมื่อคุณพยายามเปลี่ยนแปลงสิทธิ์บนโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="0b8b4-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="0b8b4-111">ดูบทความต่อไปนี้สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="0b8b4-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="0b8b4-112">ไม่สามารถใช้สิทธิ์ไปยังโฟลเดอร์สาธารณะโฟลเดอร์ย่อยใน EAC</span><span class="sxs-lookup"><span data-stu-id="0b8b4-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="0b8b4-113">ข้อผิดพลาด "กล่องจดหมายไม่พบในฟอเรสต์ภายในเครื่อง"</span><span class="sxs-lookup"><span data-stu-id="0b8b4-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
