---
title: การจัดการรายการที่อยู่ส่วนกลางขององค์กรและสมุดรายชื่อแบบออฟไลน์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022670"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="5e91d-102">การจัดการรายชื่อส่วนกลางขององค์กร (GAL) และสมุดรายชื่อแบบออฟไลน์ (OAB)</span><span class="sxs-lookup"><span data-stu-id="5e91d-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="5e91d-103">รายการที่อยู่ส่วนกลาง (GAL) คือ รายการของวัตถุที่เปิดใช้งานจดหมาย (ผู้รับชนิดใดๆ ที่สามารถรับอีเมล) ในองค์กร</span><span class="sxs-lookup"><span data-stu-id="5e91d-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="5e91d-104">หนึ่ง GAL ถูกสร้างขึ้นโดยอัตโนมัติในทุกองค์กร</span><span class="sxs-lookup"><span data-stu-id="5e91d-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="5e91d-105">คุณสามารถสร้าง GALs เพิ่มเติมเพื่อแยกผู้ใช้ตามองค์กรหรือสถานที่ แต่ผู้ใช้คนเดียวสามารถดูและใช้ GAL ได้ครั้งละหนึ่งรายเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="5e91d-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="5e91d-106">ไคลเอ็นต์อีเมลบางโปรแกรม เช่น Outlook สําหรับ Windows ดาวน์โหลด GAL สําหรับใช้แบบออฟไลน์</span><span class="sxs-lookup"><span data-stu-id="5e91d-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="5e91d-107">ซึ่งเรียกว่าสมุดรายชื่อแบบออฟไลน์ (OAB)</span><span class="sxs-lookup"><span data-stu-id="5e91d-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="5e91d-108">ใน Exchange แบบออนไลน์ OAB มีการปรับปรุงเพียงครั้งเดียวทุก 8 ชั่วโมง และจากนั้น ไคลเอนต์ต้องดาวน์โหลดการปรับปรุงสําเนา OAB ภายในเครื่องของตนเอง</span><span class="sxs-lookup"><span data-stu-id="5e91d-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="5e91d-109">การเปลี่ยนแปลงใด ๆ ของผู้รับต้องแรกสามารถมองเห็นได้ใน GAL ในภายหลังทําให้ OAB</span><span class="sxs-lookup"><span data-stu-id="5e91d-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="5e91d-110">ต่อไปนี้เป็นขั้นตอนบางส่วนที่ใช้กันทั่วไป GAL และ OAB:</span><span class="sxs-lookup"><span data-stu-id="5e91d-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="5e91d-111">ด้วยเหตุผลหลายประการ คุณอาจต้องการให้วัตถุบางวัตถุถูกซ่อนจาก GAL</span><span class="sxs-lookup"><span data-stu-id="5e91d-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="5e91d-112">กรุณาดู[ซ่อนผู้รับจากรายการที่อยู่](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)</span><span class="sxs-lookup"><span data-stu-id="5e91d-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="5e91d-113">ถ้าคุณต้องการกําหนดมุมมองที่ผู้ใช้กําหนดเองของ GAL ขององค์กร ให้ดูที่[นโยบายสมุดรายชื่อใน Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies)</span><span class="sxs-lookup"><span data-stu-id="5e91d-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="5e91d-114">[สร้างสมุดรายชื่อส่วนกลางในการแลกเปลี่ยนแบบออนไลน์](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)และเรียนรู้วิธีการทํางานกับสิทธิ์ GAL ดู[รายการที่อยู่ใน Exchange แบบออนไลน์](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)</span><span class="sxs-lookup"><span data-stu-id="5e91d-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="5e91d-115">โปรดทราบว่าถ้าคุณสร้าง GALs ใหม่ คุณอาจต้องการสร้าง OAB ใหม่</span><span class="sxs-lookup"><span data-stu-id="5e91d-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="5e91d-116">ดู[ขั้นตอนสมุดรายชื่อแบบออฟไลน์](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)</span><span class="sxs-lookup"><span data-stu-id="5e91d-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
