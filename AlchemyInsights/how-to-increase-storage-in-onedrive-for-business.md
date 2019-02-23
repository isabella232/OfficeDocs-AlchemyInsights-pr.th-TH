---
title: วิธีการเพิ่มการจัดเก็บข้อมูลใน OneDrive สำหรับธุรกิจ
ms.author: kirks
author: Techwriter40
ms.date: 12/14/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 693e7607f557f2586bf3debda8e4b7fdb04cf143
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207776"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="cdc4d-102">วิธีการเพิ่มการจัดเก็บข้อมูลใน OneDrive สำหรับธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="cdc4d-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="cdc4d-103">เมื่อต้องการเปลี่ยนเก็บข้อมูลเริ่มต้นสำหรับผู้ใช้ OneDrive ที่มีอยู่ และใหม่:</span><span class="sxs-lookup"><span data-stu-id="cdc4d-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="cdc4d-104">ไป[หน้าการจัดเก็บของศูนย์ admin OneDrive](https://admin.onedrive.com/?v=StorageSettings)และจากนั้น ป้อนยอดเงินใหม่ในกิกะไบต์</span><span class="sxs-lookup"><span data-stu-id="cdc4d-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>
    
<span data-ttu-id="cdc4d-p101">การตั้งค่าพื้นที่จัดเก็บข้อมูลนี้นำไปใช้กับผู้ใช้ทั้งหมดที่คุณไม่ได้ตั้งค่าขีดจำกัดการจัดเก็บเฉพาะ เมื่อต้องการเปลี่ยนพื้นที่การจัดเก็บสำหรับผู้ใช้บางคน คุณจำเป็นต้องใช้ Microsoft PowerShell สำหรับข้อมูลเกี่ยวกับวิธีการทำเช่นนี้ ดู[เปลี่ยนพื้นที่จัดเก็บ OneDrive ของผู้ใช้โดยใช้ PowerShell](https://go.microsoft.com/fwlink/?linkid=866402)</span><span class="sxs-lookup"><span data-stu-id="cdc4d-p101">This storage space setting applies to all users for whom you haven't set specific storage limits. To change the storage space for specific users, you need to use Microsoft PowerShell. For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span> 
  
 <span data-ttu-id="cdc4d-p102">**หมายเหตุ**: ดูเหมือนว่าคุณไม่ได้วางแผนที่มีการจัดเก็บไม่จำกัด สำหรับข้อมูลเกี่ยวกับการเก็บข้อมูลที่มาพร้อมกับแต่ละแผน ดู[OneDrive สำหรับคำอธิบายของบริการทางธุรกิจ](https://go.microsoft.com/fwlink/p/?LinkID=826071)</span><span class="sxs-lookup"><span data-stu-id="cdc4d-p102">**NOTE**: It looks like you don't have a plan that includes unlimited storage. For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="cdc4d-110">เมื่อต้องการเพิ่มการจัดเก็บข้อมูลของคุณใน OneDrive สำหรับธุรกิจ เลือกแผนการ Office 365 ที่มี**OneDrive สำหรับธุรกิจแผน 2**หรือ**E3 องค์กร 365 Office**อย่างใดอย่างหนึ่ง</span><span class="sxs-lookup"><span data-stu-id="cdc4d-110">To increase your storage in OneDrive for Business, choose an Office 365 plan that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="cdc4d-111">เมื่อต้องการเปลี่ยนแผน ใน Microsoft 365 admin ศูนย์ ไป**เรียกเก็บเงิน**\>ที่**บอกรับเป็นสมาชิก**และจากนั้น เลือก**สลับแผน**</span><span class="sxs-lookup"><span data-stu-id="cdc4d-111">To change plans, in the Microsoft 365 admin center, go to **Billing** \> **Subscriptions**, and then choose **Switch plans.**</span></span>
  
<span data-ttu-id="cdc4d-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการสลับแผนและ OneDrive สำหรับเก็บข้อมูลทางธุรกิจ ดู[สลับไปยัง Office 365 แตกต่างกันสำหรับแผนทางธุรกิจ](https://go.microsoft.com/fwlink/?LinkId=2031117)และ[OneDrive สำหรับคำอธิบายของบริการทางธุรกิจ](https://go.microsoft.com/fwlink/?LinkId-2031122)</span><span class="sxs-lookup"><span data-stu-id="cdc4d-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Office 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/?LinkId-2031122).</span></span>
  

