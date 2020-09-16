---
title: ๒๔๙๑ข้อความอีเมลการแจ้งเตือนจาก ' Phish ที่จัดส่งเนื่องจากนโยบายของผู้เช่าหรือการแทนที่ผู้ใช้
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728630"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="d6b96-102">การแจ้งเตือนข้อความอีเมลจาก ' Phish ที่จัดส่งเนื่องจากนโยบายผู้เช่าหรือการแทนที่ผู้ใช้ '</span><span class="sxs-lookup"><span data-stu-id="d6b96-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="d6b96-103">นโยบายการแจ้งเตือนเริ่มต้นที่ชื่อว่า "Phish จัดส่งเนื่องจากผู้เช่าหรือการแทนที่ผู้ใช้" ถูกยกเลิกไปยังผู้เช่าที่มีสิทธิ์การใช้งาน Office ๓๖๕ ATP P1 และ P2</span><span class="sxs-lookup"><span data-stu-id="d6b96-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="d6b96-104">ถ้าคุณได้รับการแจ้งเตือนนี้ต่อไปนี้เป็นขั้นตอนในการตรวจสอบ:</span><span class="sxs-lookup"><span data-stu-id="d6b96-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="d6b96-105">จากข้อความแจ้งเตือนให้คลิก **ดูการแจ้งเตือน** เพื่อไปยังหน้าการ **แจ้งเตือน** ในศูนย์การรักษาความปลอดภัย & การปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="d6b96-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="d6b96-106">เลือกการแจ้งเตือนเพื่อดูตัวเลือกเพื่อ**ดูรายการข้อความ**หรือ**ดูข้อความใน Explorer**</span><span class="sxs-lookup"><span data-stu-id="d6b96-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="d6b96-107">ทั้งสองตัวเลือกเหล่านี้จะนำคุณไปยังรายละเอียดของข้อความซึ่งรวมถึง ID ข้อความ</span><span class="sxs-lookup"><span data-stu-id="d6b96-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="d6b96-108">โปรดสังเกตว่าลิงก์ของภัยคุกคาม Explorer จะกรองข้อความที่ตรงกับเกณฑ์การแจ้งเตือนโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="d6b96-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="d6b96-109">คุณอาจจำเป็นต้องปรับตัวกรองวันที่ในภัยคุกคาม Explorer</span><span class="sxs-lookup"><span data-stu-id="d6b96-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="d6b96-110">ข้อความฟิชชิ่งถูกส่งไปเนื่องจากการแทนที่กำหนดค่าด้วยตนเอง:</span><span class="sxs-lookup"><span data-stu-id="d6b96-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="d6b96-111">ผู้ส่งที่ได้รับอนุญาตหรือตั้งค่าโดเมนโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d6b96-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="d6b96-112">ผู้ส่งที่ได้รับอนุญาตหรือตั้งค่าโดเมนโดยผู้ดูแลระบบในนโยบายการป้องกันสแปม</span><span class="sxs-lookup"><span data-stu-id="d6b96-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="d6b96-113">ที่อยู่ IP ที่ได้รับอนุญาตในนโยบายตัวกรองการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="d6b96-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="d6b96-114">กฎโฟลว์จดหมาย (หรือที่เรียกว่ากฎการขนส่ง) ที่ได้รับการกำหนดค่าให้อนุญาตข้อความใน</span><span class="sxs-lookup"><span data-stu-id="d6b96-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="d6b96-115">ถ้าคุณเชื่อว่าข้อความถูกทำเครื่องหมายเป็น phish อย่างไม่ถูกต้องให้ใช้ [Add-in ข้อความรายงาน](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) ของ Outlook เพื่อส่งตัวอย่างข้อความไปยังไมโครซอฟท์</span><span class="sxs-lookup"><span data-stu-id="d6b96-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
