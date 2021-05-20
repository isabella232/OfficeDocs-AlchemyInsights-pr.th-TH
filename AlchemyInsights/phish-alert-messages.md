---
title: 2491 ข้อความแจ้งเตือนข้อความอีเมลจากนโยบาย 'ส่งโดย Phish เนื่องจากผู้เช่าหรือการแทนที่ผู้ใช้'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544597"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="93824-102">การแจ้งเตือนข้อความอีเมลจากนโยบาย 'ส่งโดย Phish เนื่องจากผู้เช่าหรือการแทนที่ผู้ใช้'</span><span class="sxs-lookup"><span data-stu-id="93824-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="93824-103">นโยบายการแจ้งเตือนเริ่มต้นที่มีชื่อว่า "ส่งโดย Phish เนื่องจากผู้เช่าหรือการแทนที่ผู้ใช้" ได้เปิดให้ผู้เช่าใช้งานกับ Microsoft Defender Office 365สิทธิ์การใช้งาน P1 และ P2 แล้ว</span><span class="sxs-lookup"><span data-stu-id="93824-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="93824-104">ถ้าคุณได้รับการแจ้งเตือนนี้ ต่อไปนี้คือขั้นตอนในการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="93824-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="93824-105">จากข้อความแจ้งเตือน ให้คลิก ดู **การแจ้งเตือน เพื่อ** ไปที่หน้า **การแจ้งเตือน** ใน ศูนย์การรักษา&การปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="93824-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="93824-106">เลือกการแจ้งเตือนเพื่อดูตัวเลือกในการ **ดูรายการข้อความ หรือ\*\*\*\*ดูข้อความใน Explorer**</span><span class="sxs-lookup"><span data-stu-id="93824-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="93824-107">ตัวเลือกทั้งสองตัวเลือกจะพาคุณไปยังรายละเอียดของข้อความ ซึ่งรวมถึง ID ข้อความ</span><span class="sxs-lookup"><span data-stu-id="93824-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="93824-108">โปรดทราบว่าลิงก์ Threat Explorer จะกรองข้อความที่ตรงกับเกณฑ์การแจ้งเตือนโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="93824-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="93824-109">คุณอาจต้องปรับตัวกรองวันที่ใน Threat Explorer</span><span class="sxs-lookup"><span data-stu-id="93824-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="93824-110">ข้อความฟิชชิ่งถูกส่งเนื่องจากการแทนที่ที่กําหนดค่าด้วยตนเอง:</span><span class="sxs-lookup"><span data-stu-id="93824-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="93824-111">ผู้ส่งหรือโดเมนที่อนุญาตที่ตั้งค่าโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="93824-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="93824-112">ผู้ส่งหรือโดเมนที่อนุญาตที่ตั้งค่าโดยผู้ดูแลระบบในนโยบายการป้องกันสแปม</span><span class="sxs-lookup"><span data-stu-id="93824-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="93824-113">ที่อยู่ IP ที่อนุญาตในนโยบายตัวกรองการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="93824-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="93824-114">กฎล.ก.ล.ต. จดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน) ที่ถูกกําหนดค่าให้อนุญาตข้อความ</span><span class="sxs-lookup"><span data-stu-id="93824-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="93824-115">ถ้าคุณเชื่อว่าข้อความถูกระบุว่า Phish ไม่ถูกต้อง ให้ใช้[add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)รายงานOutlook เพื่อส่งตัวอย่างข้อความไปยัง Microsoft</span><span class="sxs-lookup"><span data-stu-id="93824-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
