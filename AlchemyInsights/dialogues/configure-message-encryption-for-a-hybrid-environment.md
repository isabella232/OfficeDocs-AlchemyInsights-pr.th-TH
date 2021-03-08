---
title: กําหนดค่าการเข้ารหัสลับข้อความในสภาพแวดล้อมแบบไฮบริด
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526604"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="9ce61-102">กําหนดค่าการเข้ารหัสลับข้อความในสภาพแวดล้อมแบบไฮบริด</span><span class="sxs-lookup"><span data-stu-id="9ce61-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="9ce61-103">For hybrid Exchange environments, on-premises users can sended email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9ce61-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="9ce61-104">เมื่อต้องการเข้ารหัสลับอีเมลโดยใช้ OME ให้ปฏิบัติตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="9ce61-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="9ce61-105">ใช้ตัวช่วยสร้าง [การกําหนดค่า](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) แบบไฮบริดเพื่อตั้งค่าสภาพแวดล้อมแบบไฮบริดของคุณ</span><span class="sxs-lookup"><span data-stu-id="9ce61-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="9ce61-106">ไม่ต้องมีขั้นตอนพิเศษในการตั้งค่าการเข้ารหัสลับ</span><span class="sxs-lookup"><span data-stu-id="9ce61-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="9ce61-107">[ตั้งค่ากฎของลโฟลว์จดหมายของคุณ](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) การเข้ารหัสลับแบบที่คุณมักจะใช้ตามปกติ</span><span class="sxs-lookup"><span data-stu-id="9ce61-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


