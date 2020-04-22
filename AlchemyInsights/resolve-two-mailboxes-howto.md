---
title: 1374 แก้ไขกล่องจดหมายที่สอง howto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1374"
- "2692"
- "3500014"
ms.assetid: 8bf1a8f2-58ef-4697-b9c0-be340de96bfe
ms.openlocfilehash: 95d85d7737ae0684b2a2c017134104bd377695f1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722551"
---
# <a name="a-user-has-two-mailboxes"></a><span data-ttu-id="34695-102">ผู้ใช้มีกล่องจดหมายที่สอง</span><span class="sxs-lookup"><span data-stu-id="34695-102">A user has two mailboxes</span></span>

<span data-ttu-id="34695-103">สภาพแวดล้อมไฮบริดสลีที่ใช้ Azure Active Directory เชื่อมต่อ (AAD เชื่อมต่อ) หรือ DirSync อาจตั้งใจทําให้ผู้ใช้มีกล่องจดหมายที่สอง: หนึ่งในสถานที่ และหนึ่งในเมฆ</span><span class="sxs-lookup"><span data-stu-id="34695-103">Hybrid environments that use Azure Active Directory Connect (AAD Connect) or DirSync might accidentally cause a user to have two mailboxes: one on-premises, and one in the cloud.</span></span> <span data-ttu-id="34695-104">กล่องจดหมายที่ซ้ํากันอาจถูกสร้างขึ้นในสถานที่ใดสถานที่หนึ่ง</span><span class="sxs-lookup"><span data-stu-id="34695-104">A duplicate mailbox could be created in either place.</span></span>

<span data-ttu-id="34695-105">เมื่อต้องการแก้ไขปัญหานี้ ให้ดูที่[วิธีการกู้คืนเมื่อกล่องจดหมายที่มีอยู่ในทั้งการแลกเปลี่ยนแบบออนไลน์ และในสถาน](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises)</span><span class="sxs-lookup"><span data-stu-id="34695-105">To resolve this issue, see [How to recover when a mailbox exists in both Exchange Online and on-premises](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises).</span></span> <span data-ttu-id="34695-106">ถ้าคุณต้องการเรียนรู้เพิ่มเติมเกี่ยวกับวิธีการหลีกเลี่ยงปัญหานี้เกิดขึ้นในอนาคต ให้ดูที่[ผู้ใช้ของฉันมีกล่องจดหมายทั้งในสถานที่และใน Exchange Online ช่วยเหลือ!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span><span class="sxs-lookup"><span data-stu-id="34695-106">If you want to learn more about how to avoid this from happening in the future, see [My user has a mailbox both on-premises and in Exchange Online. Help!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span></span>
