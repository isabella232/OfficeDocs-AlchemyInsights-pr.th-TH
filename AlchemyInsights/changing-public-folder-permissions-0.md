---
title: การเปลี่ยนสิทธิ์ของโฟลเดอร์สาธารณะ
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
ms.openlocfilehash: 9d043e81b66cea1fcb985b0e1e79078409ba0b93
ms.sourcegitcommit: f23c39009d988228213fdb2bb7350bf4a0194194
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/11/2020
ms.locfileid: "41022216"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="ff829-102">การเปลี่ยนสิทธิ์ของโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="ff829-102">Changing public folder permissions</span></span>

<span data-ttu-id="ff829-103">สิทธิ์ของโฟลเดอร์สาธารณะสามารถเปลี่ยนแปลงได้โดยผู้ใช้และผู้ดูแลระบบใน Outlook</span><span class="sxs-lookup"><span data-stu-id="ff829-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="ff829-104">ผู้ดูแลระบบยังสามารถควบคุมสิทธิ์จากศูนย์ดูแล Exchange (EAC), โดยทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ff829-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="ff829-105">ในศูนย์การจัดการ Microsoft ๓๖๕ไปที่**ศูนย์** \>ดูแลการ**แลกเปลี่ยน**</span><span class="sxs-lookup"><span data-stu-id="ff829-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="ff829-106">เลือก**โฟลเดอร์สาธารณะ**</span><span class="sxs-lookup"><span data-stu-id="ff829-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="ff829-107">คุณสามารถเปลี่ยนแปลงสิทธิ์สำหรับแต่ละโฟลเดอร์สาธารณะได้โดยการกำหนดกลุ่มความปลอดภัยให้กับสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="ff829-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="ff829-108">ผู้ใช้ต้องมีสิทธิ์ของเจ้าของในโฟลเดอร์เพื่อให้ผู้ใช้สามารถเปลี่ยนแปลงสิทธิ์ของโฟลเดอร์สาธารณะได้</span><span class="sxs-lookup"><span data-stu-id="ff829-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

> [!NOTE]
> <span data-ttu-id="ff829-109">มีปัญหาที่ทราบหลายอย่างที่คุณอาจพบเมื่อคุณพยายามที่จะเปลี่ยนแปลงสิทธิ์บนโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="ff829-109">There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="ff829-110">ดูบทความต่อไปนี้สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="ff829-110">See the following articles for more information.</span></span>
>
> [<span data-ttu-id="ff829-111">ไม่สามารถนำการอนุญาตไปใช้กับโฟลเดอร์ย่อย public folder ใน EAC</span><span class="sxs-lookup"><span data-stu-id="ff829-111">Can’t apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)
>
> [<span data-ttu-id="ff829-112">ข้อผิดพลาด "กล่องจดหมายไม่พบในฟอเรสต์ท้องถิ่น" เมื่อคุณเข้าถึงโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="ff829-112">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
