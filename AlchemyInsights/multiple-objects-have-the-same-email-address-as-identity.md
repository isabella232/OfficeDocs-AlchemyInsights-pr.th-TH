---
title: วัตถุหลายวัตถุมีที่อยู่อีเมลเดียวกันกับข้อมูลเฉพาะตัว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724634"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="5d9ea-102">วัตถุหลายวัตถุมีที่อยู่อีเมลเดียวกันกับข้อมูลเฉพาะตัว</span><span class="sxs-lookup"><span data-stu-id="5d9ea-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="5d9ea-103">**วัตถุหลายวัตถุ**</span><span class="sxs-lookup"><span data-stu-id="5d9ea-103">**Multiple objects**</span></span>

<span data-ttu-id="5d9ea-104">หนึ่งในสาเหตุทั่วไปของข้อผิดพลาดนี้ไม่สามารถกำหนดเส้นทางการร้องขอการเข้าถึงเว็บ Outlook อย่างถูกต้องในการแสดงตนของวัตถุหลายวัตถุที่มีที่อยู่อีเมลเดียวกันกับข้อมูลเฉพาะตัว</span><span class="sxs-lookup"><span data-stu-id="5d9ea-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="5d9ea-105">เมื่อต้องการค้นหาวัตถุเหล่านี้ให้เรียกใช้คำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="5d9ea-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="5d9ea-106">· รับผู้รับ <email address></span><span class="sxs-lookup"><span data-stu-id="5d9ea-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="5d9ea-107">· รับผู้ใช้ <email address></span><span class="sxs-lookup"><span data-stu-id="5d9ea-107">· Get-User <email address></span></span>

<span data-ttu-id="5d9ea-108">· รับผู้ใช้ <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="5d9ea-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="5d9ea-109">· รับที่ติดต่อ <email address></span><span class="sxs-lookup"><span data-stu-id="5d9ea-109">· Get-Contact <email address></span></span>

<span data-ttu-id="5d9ea-110">· รับ-กล่องจดหมาย <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="5d9ea-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="5d9ea-111">· รับ-กล่องจดหมาย <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="5d9ea-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="5d9ea-112">· รับ-กล่องจดหมาย <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="5d9ea-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="5d9ea-113">เมื่อต้องการแก้ไขปัญหานี้ให้เอาวัตถุออกหลายวัตถุด้วยข้อมูลเฉพาะตัวอีเมลเดียวกันและตรวจสอบให้แน่ใจว่ามีวัตถุเดียวที่มีข้อมูลเฉพาะตัวของอีเมลที่ระบุและชนิดของผู้รับเป็น UserMailbox</span><span class="sxs-lookup"><span data-stu-id="5d9ea-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="5d9ea-114">**ใช้ที่อยู่เดียวกันสำหรับกล่องจดหมายธุรกิจและผู้บริโภค**</span><span class="sxs-lookup"><span data-stu-id="5d9ea-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="5d9ea-115">สาเหตุอีกประการหนึ่งคือเมื่อใช้ที่อยู่เดียวกันสำหรับกล่องจดหมายธุรกิจและผู้บริโภค</span><span class="sxs-lookup"><span data-stu-id="5d9ea-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="5d9ea-116">ในกรณีนี้ผู้ใช้ต้องเปลี่ยนนามแฝงผู้ใช้หลักของพวกเขาจนกว่า Cafe จะสนับสนุนสถานการณ์นี้</span><span class="sxs-lookup"><span data-stu-id="5d9ea-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="5d9ea-117">นี่เป็นข้อผิดพลาดถาวรที่ไม่หายไปโดยไม่มีการแทรกแซง</span><span class="sxs-lookup"><span data-stu-id="5d9ea-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="5d9ea-118">สำหรับรายละเอียดให้ดู[ที่เปลี่ยนที่อยู่อีเมลหรือหมายเลขโทรศัพท์สำหรับบัญชี Microsoft ของคุณ](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)</span><span class="sxs-lookup"><span data-stu-id="5d9ea-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>