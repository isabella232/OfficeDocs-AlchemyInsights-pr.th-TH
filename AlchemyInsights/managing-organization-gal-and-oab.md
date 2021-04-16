---
title: การจัดการสมุดรายชื่อส่วนกลางขององค์กรและสมุดรายชื่อแบบออฟไลน์
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794851"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="56bf3-102">การจัดการสมุดรายชื่อส่วนกลาง (GAL) และสมุดรายชื่อแบบออฟไลน์ (OAB) ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="56bf3-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="56bf3-103">สมุดรายชื่อส่วนกลาง (GAL) คือรายการของวัตถุที่เปิดใช้งานจดหมาย (ชนิดของผู้รับใดๆ ที่สามารถรับอีเมล) ในองค์กร</span><span class="sxs-lookup"><span data-stu-id="56bf3-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="56bf3-104">GAL หนึ่งรายการจะถูกสร้างขึ้นโดยอัตโนมัติในทุกองค์กร</span><span class="sxs-lookup"><span data-stu-id="56bf3-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="56bf3-105">คุณสามารถสร้าง GALs เพิ่มเติมเพื่อแยกผู้ใช้ตามองค์กรหรือสถานที่ แต่ผู้ใช้คนเดียวสามารถดูและใช้ GAL ได้ทีละหนึ่งรายการเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="56bf3-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="56bf3-106">ไคลเอ็นต์อีเมลบางตัว เช่น Outlook for Windows ให้ดาวน์โหลด GAL เพื่อใช้แบบออฟไลน์</span><span class="sxs-lookup"><span data-stu-id="56bf3-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="56bf3-107">ซึ่งเรียกว่าสมุดรายชื่อแบบออฟไลน์ (OAB)</span><span class="sxs-lookup"><span data-stu-id="56bf3-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="56bf3-108">ใน Exchange Online OAB จะถูกอัปเดตทุกๆ 8 ชั่วโมงเท่านั้น และไคลเอ็นต์ต้องดาวน์โหลดเพื่ออัปเดตสําเนา OAB ภายในเครื่องของตน</span><span class="sxs-lookup"><span data-stu-id="56bf3-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="56bf3-109">การเปลี่ยนแปลงใดๆ ของผู้รับจะต้องมองเห็นได้ใน GAL ก่อนเพื่อเปลี่ยนเป็น OAB ในภายหลัง</span><span class="sxs-lookup"><span data-stu-id="56bf3-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="56bf3-110">ต่อไปนี้คือขั้นตอน GAL และ OAB ที่ใช้บ่อย:</span><span class="sxs-lookup"><span data-stu-id="56bf3-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="56bf3-111">ด้วยเหตุผลหลายประการ คุณอาจต้องการซ่อนวัตถุบางอย่างจาก GAL</span><span class="sxs-lookup"><span data-stu-id="56bf3-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="56bf3-112">โปรดดูที่ [ซ่อนผู้รับจากรายการ](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)ที่อยู่</span><span class="sxs-lookup"><span data-stu-id="56bf3-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="56bf3-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="56bf3-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="56bf3-114">[สร้างสมุดรายชื่อส่วนกลางใน Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)และเมื่อต้องการเรียนรู้วิธีใช้งานกับสิทธิ์ GAL ให้ดู[รายการที่อยู่ใน Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)</span><span class="sxs-lookup"><span data-stu-id="56bf3-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="56bf3-115">โปรดทราบว่าถ้าคุณสร้าง GALs ใหม่ คุณอาจต้องการสร้าง OAB ใหม่</span><span class="sxs-lookup"><span data-stu-id="56bf3-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="56bf3-116">ดู [กระบวนงานสมุดรายชื่อ](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)แบบออฟไลน์</span><span class="sxs-lookup"><span data-stu-id="56bf3-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
