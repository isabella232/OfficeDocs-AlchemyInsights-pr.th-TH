---
title: การเปลี่ยนการตั้งค่าการควบคุมปริมาณ EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 415990669bafb2262c558749b64385a91d159226
ms.sourcegitcommit: 61308045a58252764f6378bbeb8802b6d2ff6c0b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/08/2020
ms.locfileid: "46596802"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="53690-102">การเปลี่ยนการตั้งค่าการควบคุมปริมาณ EWS</span><span class="sxs-lookup"><span data-stu-id="53690-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="53690-103">โปรดเรียกใช้การทดสอบอัตโนมัติของเราซึ่งจะช่วยให้คุณสามารถปรับเปลี่ยนนโยบายการควบคุมปริมาณของ EWS สำหรับระยะเวลาการโยกย้ายของคุณ</span><span class="sxs-lookup"><span data-stu-id="53690-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span>

<span data-ttu-id="53690-104">โปรดทราบว่าการเปลี่ยนแปลงนโยบายการควบคุมปริมาณ EWS จะไม่มีผลต่อการโยกย้ายชนิดต่อไปนี้ (โดยใช้เครื่องมือของ Microsoft): แบบไฮบริด, แบบย่อ/แบบ (RPC/HTTP), IMAP, G Suite, โฟลเดอร์สาธารณะหรือบริการนำเข้า PST</span><span class="sxs-lookup"><span data-stu-id="53690-104">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>