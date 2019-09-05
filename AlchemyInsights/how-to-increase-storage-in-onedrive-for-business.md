---
title: วิธีการเพิ่มพื้นที่จัดเก็บข้อมูลใน OneDrive สำหรับธุรกิจ
ms.author: pebaum
author: Techwriter40
ms.date: 12/14/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 2cf4b8c4e2cd2e5e6b91d609b34fde700c408fba
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755831"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="7cb77-102">วิธีการเพิ่มพื้นที่จัดเก็บข้อมูลใน OneDrive สำหรับธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="7cb77-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="7cb77-103">การเปลี่ยนที่เก็บเริ่มต้นสำหรับผู้ใช้ OneDrive ใหม่และที่มีอยู่:</span><span class="sxs-lookup"><span data-stu-id="7cb77-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="7cb77-104">ไปที่[หน้าเก็บข้อมูลของศูนย์การจัดการ OneDrive](https://admin.onedrive.com/?v=StorageSettings)และจากนั้นป้อนยอดเงินใหม่ในหน่วย GB</span><span class="sxs-lookup"><span data-stu-id="7cb77-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>
    
<span data-ttu-id="7cb77-105">การตั้งค่าพื้นที่จัดเก็บนี้นำไปใช้กับผู้ใช้ทุกคนที่คุณยังไม่ได้ตั้งค่าขีดจำกัดที่เก็บข้อมูลเฉพาะ</span><span class="sxs-lookup"><span data-stu-id="7cb77-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="7cb77-106">ในการเปลี่ยนแปลงพื้นที่จัดเก็บสำหรับผู้ใช้ที่เฉพาะเจาะจงคุณจำเป็นต้องใช้ Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="7cb77-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="7cb77-107">สำหรับข้อมูลเกี่ยวกับวิธีการทำเช่นนี้โปรดดูที่การ[เปลี่ยนพื้นที่จัดเก็บข้อมูล OneDrive ของผู้ใช้ของคุณโดยใช้ PowerShell](https://go.microsoft.com/fwlink/?linkid=866402)</span><span class="sxs-lookup"><span data-stu-id="7cb77-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span> 
  
 <span data-ttu-id="7cb77-108">**หมายเหตุ**: ดูเหมือนว่าคุณไม่มีแผนที่มีพื้นที่เก็บข้อมูลแบบไม่จำกัด</span><span class="sxs-lookup"><span data-stu-id="7cb77-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="7cb77-109">สำหรับข้อมูลเกี่ยวกับที่เก็บข้อมูลที่มาพร้อมกับแต่ละแผนให้ดูที่[OneDrive สำหรับคำอธิบายบริการธุรกิจ](https://go.microsoft.com/fwlink/p/?LinkID=826071)</span><span class="sxs-lookup"><span data-stu-id="7cb77-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="7cb77-110">เพื่อเพิ่มพื้นที่เก็บข้อมูลของคุณใน OneDrive สำหรับธุรกิจเลือกแผน Office ๓๖๕ที่มี**OneDrive สำหรับแผนธุรกิจ 2**หรือ**Office ๓๖๕องค์กร E3**</span><span class="sxs-lookup"><span data-stu-id="7cb77-110">To increase your storage in OneDrive for Business, choose an Office 365 plan that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="7cb77-111">เพื่อเปลี่ยนแผนในศูนย์ดูแลของ Microsoft ๓๖๕ไปที่การบอกรับเป็น**สมาชิก**การ**เรียกเก็บเงิน** \>และจากนั้นเลือก**สลับแผน**</span><span class="sxs-lookup"><span data-stu-id="7cb77-111">To change plans, in the Microsoft 365 admin center, go to **Billing** \> **Subscriptions**, and then choose **Switch plans.**</span></span>
  
<span data-ttu-id="7cb77-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการสลับแผนและ OneDrive สำหรับที่เก็บธุรกิจโปรดดูที่[สลับไปยัง Office ๓๖๕อื่นสำหรับแผนธุรกิจ](https://go.microsoft.com/fwlink/?LinkId=2031117)และการ[Onedrive สำหรับคำอธิบายบริการทางธุรกิจ](https://go.microsoft.com/fwlink/?LinkId-2031122)</span><span class="sxs-lookup"><span data-stu-id="7cb77-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Office 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/?LinkId-2031122).</span></span>
  

