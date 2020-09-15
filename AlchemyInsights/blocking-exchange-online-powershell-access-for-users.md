---
title: ๗๖๓การบล็อกการเข้าถึง PowerShell Exchange Online สำหรับผู้ใช้
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "763"
- "3500011"
ms.assetid: fcaafe9d-80ee-404b-9a70-00bc4aa5e28a
ms.openlocfilehash: 8ac61cb2c1e055c67538e39e8459b3eb56c95592
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685545"
---
# <a name="blocking-exchange-online-powershell-access-for-users"></a><span data-ttu-id="1cdda-102">การบล็อกการเข้าถึง PowerShell Exchange Online สำหรับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="1cdda-102">Blocking Exchange Online PowerShell access for users</span></span>
<span data-ttu-id="1cdda-103">ในฐานะผู้ดูแลระบบคุณจะมีความสามารถในการบล็อกการเข้าถึง Exchange Online PowerShell สำหรับผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="1cdda-103">As an admin, you have the ability to block access to Exchange Online PowerShell for your users.</span></span> <span data-ttu-id="1cdda-104">สำหรับข้อมูลเพิ่มเติมให้ดูหัวข้อต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1cdda-104">For more information, see these topics:</span></span>

- [<span data-ttu-id="1cdda-105">เปิดใช้งานหรือปิดใช้งานการเข้าถึง Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="1cdda-105">Enable or disable access to Exchange Online PowerShell</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/disable-access-to-exchange-online-powershell)

- <span data-ttu-id="1cdda-106">[กฎการเข้าถึงไคลเอ็นต์ใน Exchange Online](https://technet.microsoft.com/library/mt842508.aspx) (ค้นหาโพรโทคอ **RemotePowerShell** )</span><span class="sxs-lookup"><span data-stu-id="1cdda-106">[Client Access Rules in Exchange Online](https://technet.microsoft.com/library/mt842508.aspx) (look for the **RemotePowerShell** protocol)</span></span> 

<span data-ttu-id="1cdda-107">**หมายเหตุ**: ตามที่อธิบายไว้ในหัวข้อให้ระมัดระวังไม่ให้บล็อกการเข้าถึง Exchange Online PowerShell สำหรับผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="1cdda-107">**Note**: As the described in the topic, be careful not to block access to Exchange Online PowerShell for admins.</span></span>
