---
title: วัตถุหลายวัตถุมีที่อยู่อีเมลเดียวกันกับข้อมูลประจําตัว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439708"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="a3aba-102">วัตถุหลายวัตถุมีที่อยู่อีเมลเดียวกันกับข้อมูลประจําตัว</span><span class="sxs-lookup"><span data-stu-id="a3aba-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="a3aba-103">**วัตถุหลายวัตถุ**</span><span class="sxs-lookup"><span data-stu-id="a3aba-103">**Multiple objects**</span></span>

<span data-ttu-id="a3aba-104">หนึ่งในสาเหตุทั่วไปของข้อผิดพลาดนี้จะไม่สามารถกําหนดเส้นทางการร้องขอ Outlook Web Access ได้อย่างถูกต้องในสถานะการมีอยู่ของวัตถุหลายวัตถุที่มีที่อยู่อีเมลเดียวกันเป็นข้อมูลประจําตัว</span><span class="sxs-lookup"><span data-stu-id="a3aba-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="a3aba-105">เมื่อต้องการค้นหาวัตถุเหล่านี้ ให้เรียกใช้คําสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a3aba-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="a3aba-106">· รับผู้รับ<email address></span><span class="sxs-lookup"><span data-stu-id="a3aba-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="a3aba-107">· รับผู้ใช้<email address></span><span class="sxs-lookup"><span data-stu-id="a3aba-107">· Get-User <email address></span></span>

<span data-ttu-id="a3aba-108">· รับผู้ใช้ <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="a3aba-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="a3aba-109">· ติดต่อรับ<email address></span><span class="sxs-lookup"><span data-stu-id="a3aba-109">· Get-Contact <email address></span></span>

<span data-ttu-id="a3aba-110">· รับกล่องจดหมาย <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="a3aba-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="a3aba-111">· รับกล่องจดหมาย <email address> -รวมรวมการติดแท็ก</span><span class="sxs-lookup"><span data-stu-id="a3aba-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="a3aba-112">· รับกล่องจดหมาย <email address> -ไม่ได้ใช้งานกล่องจดหมายเดียว</span><span class="sxs-lookup"><span data-stu-id="a3aba-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="a3aba-113">เมื่อต้องการแก้ไขปัญหา ลบวัตถุหลายวัตถุ ด้วยรหัสประจําตัวอีเมลเดียวกัน และให้แน่ใจว่า ไม่มีวัตถุเดียว กับรหัสประจําตัวอีเมลเฉพาะ และว่า ชนิดผู้รับเป็น UserMailbox</span><span class="sxs-lookup"><span data-stu-id="a3aba-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="a3aba-114">**ที่อยู่เดียวกันจะใช้สําหรับกล่องจดหมายของธุรกิจและผู้บริโภค**</span><span class="sxs-lookup"><span data-stu-id="a3aba-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="a3aba-115">สาเหตุก็คือเมื่อมีใช้ที่อยู่เดียวกันสําหรับธุรกิจและกล่องจดหมายของผู้บริโภค</span><span class="sxs-lookup"><span data-stu-id="a3aba-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="a3aba-116">ในกรณีนี้ ผู้ใช้ต้องเปลี่ยนนามแฝงของผู้บริโภคหลักจนกว่า Cafe สนับสนุนสถานการณ์สมมตินี้</span><span class="sxs-lookup"><span data-stu-id="a3aba-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="a3aba-117">นี่คือข้อผิดพลาดถาวรที่ไม่หายไปโดยไม่มีการแทรกแซง</span><span class="sxs-lookup"><span data-stu-id="a3aba-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="a3aba-118">โปรดดูรายละเอียดที่[เปลี่ยนที่อยู่อีเมลหรือหมายเลขโทรศัพท์สําหรับบัญชี Microsoft ของคุณ](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)</span><span class="sxs-lookup"><span data-stu-id="a3aba-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>