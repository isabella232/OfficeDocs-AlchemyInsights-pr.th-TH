---
title: นโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange ไม่ใช้งาน
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952247"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="735dd-102">นโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange</span><span class="sxs-lookup"><span data-stu-id="735dd-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="735dd-103">ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบการตั้งค่าที่กล่าวถึงด้านล่างโดยอัตโนมัติ ให้เลือกปุ่ม ย้อนกลับ < ที่ด้านบนของหน้านี้ จากนั้นใส่ที่อยู่อีเมลของผู้ใช้ที่มีปัญหากับนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="735dd-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="735dd-104">ถ้าคุณมีปัญหากับนโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange จะไม่ใช้กับกล่องจดหมายหรือรายการที่ไม่ได้ย้ายไปยังกล่องจดหมายเก็บถาวร ให้ตรวจสอบดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="735dd-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="735dd-105">**สาเหตุหลัก:**</span><span class="sxs-lookup"><span data-stu-id="735dd-105">**Root Causes:**</span></span>

- <span data-ttu-id="735dd-106">**ตัวช่วยโฟลเดอร์ที่มี** การจัดการไม่ได้ประมวลผลกล่องจดหมายของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="735dd-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="735dd-107">ตัวช่วยโฟลเดอร์ที่มีการจัดการจะพยายามประมวลผลกล่องจดหมายทั้งหมดในองค์กรระบบคลาวด์ของคุณทุกๆ 7 วัน</span><span class="sxs-lookup"><span data-stu-id="735dd-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="735dd-108">**วิธีแก้ไข:** เรียกใช้ตัวช่วยจัดการโฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="735dd-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="735dd-109">**มีการเปิดใช้งาน RetentionHold** บนกล่องจดหมายแล้ว</span><span class="sxs-lookup"><span data-stu-id="735dd-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="735dd-110">ถ้ากล่องจดหมายถูกวางไว้ใน RetentionHold นโยบายการเก็บข้อมูลบนกล่องจดหมายจะไม่ถูกประมวลผลระหว่างช่วงเวลาดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="735dd-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="735dd-111">**วิธีแก้ไข:** ตรวจสอบสถานะของการตั้งค่าการหยุดการเก็บข้อมูลและอัปเดตตามต้องการ</span><span class="sxs-lookup"><span data-stu-id="735dd-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="735dd-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="735dd-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="735dd-113">**หมายเหตุ:** ถ้ากล่องจดหมายมีขนาดเล็กกว่า 10 MB ตัวช่วยจัดการโฟลเดอร์จะไม่ประมวลผลกล่องจดหมายโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="735dd-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="735dd-114">ดูข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange ที่:</span><span class="sxs-lookup"><span data-stu-id="735dd-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="735dd-115">แท็กการเก็บข้อมูลและนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="735dd-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="735dd-116">[ใช้นโยบายการเก็บข้อมูลกับกล่องจดหมาย หรือเพิ่ม](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)[หรือเอาแท็กการเก็บข้อมูลออก](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="735dd-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="735dd-117">วิธีการระบุชนิดของการหยุดบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="735dd-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
