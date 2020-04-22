---
title: 2491แจ้งเตือนข้อความอีเมลจากนโยบาย 'Phish ที่ถูกส่งเนื่องจากผู้ใช้แทนผู้เช่าหรือผู้ใช้'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758953"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="1495a-102">แจ้งเตือนข้อความอีเมลจากนโยบาย 'ฟิชที่ถูกส่งเนื่องจากการแทนที่ผู้เช่าหรือผู้ใช้'</span><span class="sxs-lookup"><span data-stu-id="1495a-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="1495a-103">นโยบายการแจ้งเตือนเริ่มต้นที่ชื่อ "Phish ส่งเนื่องจากการแทนที่ผู้เช่าหรือผู้ใช้" ได้ถูกเปิดตัวไปยังผู้เช่าที่มีสิทธิ์การใช้งาน Office 365 ATP P1 และ P2</span><span class="sxs-lookup"><span data-stu-id="1495a-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="1495a-104">หากคุณได้รับการแจ้งเตือนนี้</span><span class="sxs-lookup"><span data-stu-id="1495a-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="1495a-105">จากข้อความแจ้งเตือน ให้คลิก**ดูการแจ้งเตือน**เพื่อไปยังหน้า**การแจ้งเตือน**ในศูนย์การปฏิบัติตามข้อกําหนดด้านความปลอดภัย &</span><span class="sxs-lookup"><span data-stu-id="1495a-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="1495a-106">เลือกการแจ้งเตือนเพื่อดูตัวเลือกในการ**ดูรายการข้อความ**หรือ**ดูข้อความใน Explorer**</span><span class="sxs-lookup"><span data-stu-id="1495a-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="1495a-107">ตัวเลือกทั้งสองนี้จะนําคุณไปยังรายละเอียดของข้อความ ซึ่งรวมถึงรหัสข้อความ</span><span class="sxs-lookup"><span data-stu-id="1495a-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="1495a-108">โปรดทราบว่าลิงก์ Threat Explorer จะกรองข้อความที่ตรงกับเกณฑ์การแจ้งเตือนโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="1495a-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="1495a-109">คุณอาจต้องปรับตัวกรองวันที่ใน Threat Explorer</span><span class="sxs-lookup"><span data-stu-id="1495a-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="1495a-110">ข้อความฟิชชิ่งถูกส่งเนื่องจากการกําหนดค่าด้วยตนเองแทน:</span><span class="sxs-lookup"><span data-stu-id="1495a-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="1495a-111">ผู้ส่งหรือโดเมนที่อนุญาตที่กําหนดโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="1495a-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="1495a-112">ผู้ส่งหรือโดเมนที่ผู้ดูแลระบบกําหนดในนโยบายการป้องกันสแปมที่ได้รับอนุญาต</span><span class="sxs-lookup"><span data-stu-id="1495a-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="1495a-113">ที่อยู่ IP ที่ได้รับอนุญาตในนโยบายการกรองการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="1495a-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="1495a-114">กฎกระแสจดหมาย (หรือที่เรียกว่ากฎการส่งผ่านข้อมูล) ที่ถูกกําหนดค่าให้อนุญาตข้อความ</span><span class="sxs-lookup"><span data-stu-id="1495a-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="1495a-115">ถ้าคุณเชื่อว่า ข้อความถูกทําเครื่องหมายว่าฟิชอย่างไม่ถูกต้อง ให้ใช้[Add-in ข้อความรายงาน](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)ของ Outlook เพื่อส่งตัวอย่างข้อความไปยัง Microsoft</span><span class="sxs-lookup"><span data-stu-id="1495a-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
