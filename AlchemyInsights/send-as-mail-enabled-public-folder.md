---
title: โฟลเดอร์สาธารณะที่เปิดใช้งาน ส่งเป็นจดหมาย ใน EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052585"
---
# <a name="sendas-mail-enabled-public-folder"></a>โฟลเดอร์สาธารณะที่เปิดใช้งาน SendAs Mail

ตัวอย่างต่อไปนี้กําหนดสิทธิ์ "ส่งเป็น" ให้กับโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย NewPF1 ให้กับผู้ใช้ Jason

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

