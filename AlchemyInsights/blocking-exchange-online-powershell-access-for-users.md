---
title: บล็อกการแลกเปลี่ยนแบบออนไลน์ PowerShell 763 การเข้าถึงสำหรับผู้ใช้
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/26/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "763"
- "3500011"
ms.assetid: fcaafe9d-80ee-404b-9a70-00bc4aa5e28a
ms.openlocfilehash: f5e432423aa2792de4c13060b94a930892710057
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517950"
---
# <a name="blocking-exchange-online-powershell-access-for-users"></a><span data-ttu-id="791d2-102">บล็อกของ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนการเข้าถึงสำหรับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="791d2-102">Blocking Exchange Online PowerShell access for users</span></span>
<span data-ttu-id="791d2-103">เป็นผู้ดูแลระบบการ คุณมีความสามารถในการบล็อกการเข้าถึงของ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนสำหรับผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="791d2-103">As an admin, you have the ability to block access to Exchange Online PowerShell for your users.</span></span> <span data-ttu-id="791d2-104">สำหรับข้อมูลเพิ่มเติม ดูหัวข้อเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="791d2-104">For more information, see these topics:</span></span>

- [<span data-ttu-id="791d2-105">เปิดใช้งาน หรือปิดใช้งานการเข้าถึงของ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="791d2-105">Enable or disable access to Exchange Online PowerShell</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/disable-access-to-exchange-online-powershell)

- <span data-ttu-id="791d2-106">[ไคลเอนต์การเข้าถึงกฎการแลกเปลี่ยนแบบออนไลน์](https://technet.microsoft.com/library/mt842508.aspx) (ค้นหาโพรโทคอล**RemotePowerShell** )</span><span class="sxs-lookup"><span data-stu-id="791d2-106">[Client Access Rules in Exchange Online](https://technet.microsoft.com/library/mt842508.aspx) (look for the **RemotePowerShell** protocol)</span></span> 

<span data-ttu-id="791d2-107">**หมายเหตุ**: ตามที่อธิบายไว้ในหัวข้อ ระวังไม่ให้บล็อกการเข้าถึงของ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนสำหรับผู้ดูแล</span><span class="sxs-lookup"><span data-stu-id="791d2-107">**Note**: As the described in the topic, be careful not to block access to Exchange Online PowerShell for admins.</span></span>
