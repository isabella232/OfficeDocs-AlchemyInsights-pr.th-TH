---
title: การจัดการรายการที่อยู่สากลขององค์กรและสมุดรายชื่อแบบออฟไลน์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a15864f34433695b61ea040abd3032d234920653
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812710"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="83190-102">การจัดการรายการที่อยู่ส่วนกลางขององค์กร (GAL) และสมุดรายชื่อแบบออฟไลน์ (OAB)</span><span class="sxs-lookup"><span data-stu-id="83190-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="83190-103">สมุดรายชื่อส่วนกลาง (GAL) คือรายการของวัตถุที่เปิดใช้งานจดหมาย (ชนิดของผู้รับใดก็ตามที่สามารถรับอีเมลได้) ในองค์กร</span><span class="sxs-lookup"><span data-stu-id="83190-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="83190-104">หนึ่ง GAL จะถูกสร้างขึ้นโดยอัตโนมัติในทุกองค์กร</span><span class="sxs-lookup"><span data-stu-id="83190-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="83190-105">คุณสามารถสร้าง GALs เพิ่มเติมเพื่อแยกผู้ใช้ตามองค์กรหรือตำแหน่งที่ตั้งแต่ผู้ใช้คนเดียวจะสามารถดูและใช้หนึ่ง GAL ในแต่ละครั้งเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="83190-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="83190-106">ไคลเอ็นต์อีเมลบางรายการเช่น Outlook สำหรับ Windows ให้ดาวน์โหลด GAL สำหรับการใช้งานแบบออฟไลน์</span><span class="sxs-lookup"><span data-stu-id="83190-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="83190-107">ซึ่งเรียกว่าสมุดรายชื่อแบบออฟไลน์ (OAB)</span><span class="sxs-lookup"><span data-stu-id="83190-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="83190-108">ใน Exchange online, OAB จะได้รับการอัปเดตเมื่อทุกๆ8ชั่วโมงแล้วไคลเอ็นต์จะต้องดาวน์โหลดเพื่ออัปเดตระเบียน OAB ภายในเครื่องของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="83190-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="83190-109">การเปลี่ยนแปลงผู้รับใดๆจะปรากฏให้เห็นใน GAL ก่อนที่จะทำให้เป็น OAB ในภายหลัง</span><span class="sxs-lookup"><span data-stu-id="83190-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="83190-110">ต่อไปนี้คือขั้นตอนการใช้งาน GAL และ OAB ที่ใช้กันทั่วไป:</span><span class="sxs-lookup"><span data-stu-id="83190-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="83190-111">ด้วยเหตุผลหลายประการคุณอาจต้องการให้วัตถุบางอย่างถูกซ่อนจาก GAL</span><span class="sxs-lookup"><span data-stu-id="83190-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="83190-112">โปรดดู[ที่ซ่อนผู้รับจากรายการที่อยู่](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)</span><span class="sxs-lookup"><span data-stu-id="83190-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="83190-113">ถ้าคุณต้องการให้กลุ่มที่เฉพาะเจาะจงของผู้ใช้มุมมองที่กำหนดเองของ GAL ขององค์กรให้ดู[ที่นโยบายสมุดรายชื่อใน Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies)</span><span class="sxs-lookup"><span data-stu-id="83190-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="83190-114">[สร้างสมุดรายชื่อส่วนกลางใน Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)และเรียนรู้วิธีการทำงานกับสิทธิ์ GAL ให้ดู[ที่รายการที่อยู่ใน Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)</span><span class="sxs-lookup"><span data-stu-id="83190-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="83190-115">โปรดทราบว่าถ้าคุณสร้าง GALs ใหม่คุณอาจต้องการสร้าง OAB ใหม่</span><span class="sxs-lookup"><span data-stu-id="83190-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="83190-116">ดู[ขั้นตอนของสมุดรายชื่อแบบออฟไลน์](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)</span><span class="sxs-lookup"><span data-stu-id="83190-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
