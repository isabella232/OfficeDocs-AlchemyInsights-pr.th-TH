---
title: วิธีเพิ่มที่เก็บข้อมูลใน OneDrive for Business
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 53eabf6c87dead3b7309c7da1f8a590940127169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780114"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="26542-102">วิธีเพิ่มที่เก็บข้อมูลใน OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="26542-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="26542-103">เมื่อต้องการเปลี่ยนที่เก็บข้อมูลเริ่มต้นสำหรับผู้ใช้ OneDrive ใหม่และผู้ใช้ที่มีอยู่:</span><span class="sxs-lookup"><span data-stu-id="26542-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="26542-104">ไปที่ [หน้าที่เก็บข้อมูลของศูนย์การจัดการ OneDrive](https://admin.onedrive.com/?v=StorageSettings)แล้วใส่จำนวนเงินใหม่ในหน่วยกิกะไบต์</span><span class="sxs-lookup"><span data-stu-id="26542-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="26542-105">การตั้งค่าพื้นที่จัดเก็บข้อมูลนี้จะนำไปใช้กับผู้ใช้ทั้งหมดที่คุณไม่ได้ตั้งค่าขีดจำกัดที่เก็บข้อมูลที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="26542-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="26542-106">เมื่อต้องการเปลี่ยนพื้นที่จัดเก็บข้อมูลสำหรับผู้ใช้ที่เฉพาะเจาะจงคุณจำเป็นต้องใช้ Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="26542-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="26542-107">สำหรับข้อมูลเกี่ยวกับวิธีการทำสิ่งนี้ให้ดูที่[เปลี่ยนพื้นที่เก็บข้อมูล OneDrive ของผู้ใช้ของคุณโดยใช้ PowerShell](https://go.microsoft.com/fwlink/?linkid=866402)</span><span class="sxs-lookup"><span data-stu-id="26542-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="26542-108">**หมายเหตุ**: ดูเหมือนว่าคุณยังไม่มีแผนที่มีที่เก็บข้อมูลแบบไม่จำกัด</span><span class="sxs-lookup"><span data-stu-id="26542-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="26542-109">สำหรับข้อมูลเกี่ยวกับที่เก็บข้อมูลที่มาพร้อมกับแต่ละแผนให้ดูที่[คำอธิบายบริการ OneDrive For Business](https://go.microsoft.com/fwlink/p/?LinkID=826071)</span><span class="sxs-lookup"><span data-stu-id="26542-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="26542-110">เมื่อต้องการเพิ่มพื้นที่จัดเก็บข้อมูลของคุณใน OneDrive for Business ให้เลือกการสมัครใช้งานที่มี**onedrive For Business Plan 2**หรือ**Office ๓๖๕ Enterprise E3**</span><span class="sxs-lookup"><span data-stu-id="26542-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="26542-111">เมื่อต้องการเปลี่ยนแผนในศูนย์การจัดการ Microsoft ๓๖๕ให้ไปที่หน้าการ**เรียกเก็บเงิน** \> **[ของผลิตภัณฑ์ของคุณ](https://go.microsoft.com/fwlink/p/?linkid=842054)** เลือกการสมัครใช้งานเพื่อเปลี่ยนแปลงแล้วเลือกแท็บการ**อัปเกรด**</span><span class="sxs-lookup"><span data-stu-id="26542-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="26542-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการสลับแผนและที่เก็บข้อมูล OneDrive for Business ให้ดูที่[สลับไปยังแผนอื่นของ Microsoft ๓๖๕สำหรับธุรกิจ](https://go.microsoft.com/fwlink/?LinkId=2031117)และ[คำอธิบายบริการ OneDrive for business](https://go.microsoft.com/fwlink/p/?LinkId-2031122)</span><span class="sxs-lookup"><span data-stu-id="26542-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>