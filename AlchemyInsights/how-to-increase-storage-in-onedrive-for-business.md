---
title: วิธีการเพิ่มที่เก็บข้อมูลใน OneDrive สําหรับธุรกิจ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: adee1c5d1ffc23f54580549ab666ee8fac579263
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/13/2020
ms.locfileid: "44063060"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="904d7-102">วิธีการเพิ่มที่เก็บข้อมูลใน OneDrive สําหรับธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="904d7-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="904d7-103">เมื่อต้องการเปลี่ยนที่เก็บข้อมูลเริ่มต้นสําหรับผู้ใช้ OneDrive ใหม่และที่มีอยู่ ให้ทําดังนี้</span><span class="sxs-lookup"><span data-stu-id="904d7-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="904d7-104">ไปที่หน้า[พื้นที่จัดเก็บ ของศูนย์การจัดการ OneDrive](https://admin.onedrive.com/?v=StorageSettings)แล้วป้อนจํานวนเงินใหม่ในหน่วย GB</span><span class="sxs-lookup"><span data-stu-id="904d7-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="904d7-105">การตั้งค่าพื้นที่จัดเก็บนี้ใช้กับผู้ใช้ทุกคนที่คุณไม่ได้ตั้งค่าขีดจํากัดของพื้นที่จัดเก็บข้อมูลที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="904d7-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="904d7-106">เมื่อต้องการเปลี่ยนพื้นที่จัดเก็บสําหรับผู้ใช้เฉพาะ</span><span class="sxs-lookup"><span data-stu-id="904d7-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="904d7-107">สําหรับข้อมูลเกี่ยวกับวิธีการทําเช่นนี้ ให้ดูที่[การเปลี่ยนพื้นที่จัดเก็บข้อมูล OneDrive ของผู้ใช้โดยใช้ PowerShell](https://go.microsoft.com/fwlink/?linkid=866402)</span><span class="sxs-lookup"><span data-stu-id="904d7-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="904d7-108">**หมายเหตุ**: ดูเหมือนว่าคุณไม่ได้มีแผนที่มีพื้นที่เก็บข้อมูลไม่ จํากัด</span><span class="sxs-lookup"><span data-stu-id="904d7-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="904d7-109">สําหรับข้อมูลเกี่ยวกับที่เก็บที่มาพร้อมกับแผนแต่ละแผน ให้ดูที่[OneDrive for Business คําอธิบายบริการ](https://go.microsoft.com/fwlink/p/?LinkID=826071)</span><span class="sxs-lookup"><span data-stu-id="904d7-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="904d7-110">เมื่อต้องการเพิ่มที่เก็บข้อมูลของคุณใน OneDrive for Business ให้เลือกการสมัครใช้งานที่มี**OneDrive สําหรับแผนธุรกิจ 2**หรือ**Office 365 Enterprise E3**</span><span class="sxs-lookup"><span data-stu-id="904d7-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="904d7-111">เมื่อต้องการเปลี่ยนแปลงแผน ใน ศูนย์การจัดการ Microsoft 365 ให้ไปที่หน้า**การเรียกเก็บเงิน** \> **[ผลิตภัณฑ์ของคุณ](https://go.microsoft.com/fwlink/p/?linkid=842054)** ให้เลือกการสมัครใช้งานที่จะเปลี่ยนแปลง แล้วเลือกแท็บ**ปรับรุ่น**</span><span class="sxs-lookup"><span data-stu-id="904d7-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="904d7-112">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการสลับแผนและ OneDrive สําหรับการจัดเก็บธุรกิจ ให้ดูที่[สลับไปยัง Microsoft 365 อื่นสําหรับแผนธุรกิจ](https://go.microsoft.com/fwlink/?LinkId=2031117)และ[OneDrive สําหรับรายละเอียดการบริการธุรกิจ](https://go.microsoft.com/fwlink/p/?LinkId-2031122)</span><span class="sxs-lookup"><span data-stu-id="904d7-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>