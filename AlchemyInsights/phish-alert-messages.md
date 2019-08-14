---
title: ข้อความอีเมลที่แจ้งเตือน 2491 จากนโยบาย 'การแทนการจัดส่งเนื่องจากผู้เช่าหรือผู้ใช้ Phish'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391580"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="da07d-102">ข้อความอีเมลการแจ้งเตือนจากนโยบาย 'การแทนการจัดส่งเนื่องจากผู้เช่าหรือผู้ใช้ Phish'</span><span class="sxs-lookup"><span data-stu-id="da07d-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="da07d-103">สะสมนโยบายแจ้งเตือนเริ่มต้นมีชื่อว่า "Phish จัดส่งเนื่องจากการแทนผู้เช่าหรือผู้ใช้" ออกไปผู้เช่ากับใบอนุญาต Office 365 ATP P1 และ P2</span><span class="sxs-lookup"><span data-stu-id="da07d-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="da07d-104">ถ้าคุณได้รับข้อความแจ้งเตือนนี้ ต่อไปนี้เป็นขั้นตอนการตรวจสอบ:</span><span class="sxs-lookup"><span data-stu-id="da07d-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="da07d-105">จากข้อความแจ้งเตือน คลิก**มุมมองการแจ้งเตือน**เมื่อต้องการไปยังเพจการ**แจ้งเตือน**ใน & ความปลอดภัยศูนย์การปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="da07d-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="da07d-106">เลือกการแจ้งเตือนเมื่อต้องการดูตัวเลือกเพื่อ**ดูรายการของข้อความ**หรือ**ดูข้อความใน Explorer**</span><span class="sxs-lookup"><span data-stu-id="da07d-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="da07d-107">ทั้งสองตัวเลือกเหล่านี้นำคุณไปรายละเอียดของข้อความ ซึ่งประกอบด้วยรหัสข้อความ</span><span class="sxs-lookup"><span data-stu-id="da07d-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="da07d-108">โปรดสังเกตว่า การคุกคาม Explorer เชื่อมโยงโดยอัตโนมัติกรองข้อความที่ตรงกับเกณฑ์การแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="da07d-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="da07d-109">คุณอาจต้องปรับเปลี่ยนตัวกรองวันที่ใน Explorer คุกคาม</span><span class="sxs-lookup"><span data-stu-id="da07d-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="da07d-110">มีการส่งข้อความฟิชชิ่งได้เนื่องจากการแทนที่ถูกกำหนดค่าด้วยตนเอง:</span><span class="sxs-lookup"><span data-stu-id="da07d-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="da07d-111">อนุญาตผู้ส่งหรือโดเมนที่กำหนด โดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="da07d-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="da07d-112">อนุญาตผู้ส่งหรือโดเมนที่ตั้งค่า โดยผู้ดูแลในนโยบายการสแปม</span><span class="sxs-lookup"><span data-stu-id="da07d-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="da07d-113">อนุญาตอยู่ IP ในการเชื่อมต่อตัวกรองนโยบาย</span><span class="sxs-lookup"><span data-stu-id="da07d-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="da07d-114">จดหมายกระแสกฎ (หรือที่เรียกอีกอย่างหนึ่งว่ากฎการขนส่ง) ที่ถูกกำหนดค่าให้อนุญาตให้มีข้อความใน</span><span class="sxs-lookup"><span data-stu-id="da07d-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="da07d-115">ถ้าคุณเชื่อว่า ข้อความถูกทำเครื่องหมายเป็น phish อย่างไม่ถูกต้อง ใช้ Outlook [add-in ของข้อความในรายงาน](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)เมื่อต้องการส่งข้อความตัวอย่างไปยัง Microsoft</span><span class="sxs-lookup"><span data-stu-id="da07d-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
