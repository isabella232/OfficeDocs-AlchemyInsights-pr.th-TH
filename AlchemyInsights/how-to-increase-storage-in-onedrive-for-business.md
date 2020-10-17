---
title: วิธีเพิ่มที่เก็บข้อมูลใน OneDrive for Business
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 676b17d47ee5071ed45e8d6022eaa82b51fc4d51
ms.sourcegitcommit: ad2d185aa9e08c27c4a1c4803b679cc4e6305703
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/16/2020
ms.locfileid: "48489044"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="7797a-102">วิธีเพิ่มที่เก็บข้อมูลใน OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="7797a-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="7797a-103">เมื่อต้องการเปลี่ยนที่เก็บข้อมูลเริ่มต้นสำหรับผู้ใช้ OneDrive ใหม่และผู้ใช้ที่มีอยู่:</span><span class="sxs-lookup"><span data-stu-id="7797a-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="7797a-104">ไปที่[หน้าที่เก็บข้อมูลของศูนย์การจัดการ OneDrive](https://admin.onedrive.com/?v=StorageSettings)แล้วใส่จำนวนเงินใหม่ใน GB จากนั้นเลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="7797a-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), enter a new amount in GB, then select **Save**.</span></span>

<span data-ttu-id="7797a-105">การตั้งค่าพื้นที่จัดเก็บข้อมูลนี้จะนำไปใช้กับผู้ใช้ทั้งหมดที่คุณไม่ได้ตั้งค่าขีดจำกัดที่เก็บข้อมูลที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="7797a-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="7797a-106">เมื่อต้องการเปลี่ยนพื้นที่จัดเก็บข้อมูลสำหรับผู้ใช้ที่เฉพาะเจาะจงให้ใช้ Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="7797a-106">To change the storage space for specific users, use Microsoft PowerShell.</span></span> <span data-ttu-id="7797a-107">สำหรับข้อมูลเกี่ยวกับวิธีการทำสิ่งนี้ให้ดูที่[เปลี่ยนพื้นที่เก็บข้อมูล OneDrive ของผู้ใช้ของคุณโดยใช้ PowerShell](https://docs.microsoft.com/onedrive/change-user-storage)</span><span class="sxs-lookup"><span data-stu-id="7797a-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://docs.microsoft.com/onedrive/change-user-storage).</span></span>

<span data-ttu-id="7797a-108">**หมายเหตุ**: ดูเหมือนว่าคุณยังไม่มีแผนที่มีที่เก็บข้อมูลแบบไม่จำกัด</span><span class="sxs-lookup"><span data-stu-id="7797a-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="7797a-109">สำหรับข้อมูลเกี่ยวกับที่เก็บข้อมูลที่มาพร้อมกับแต่ละแผนให้ดูที่[คำอธิบายบริการ OneDrive For Business](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)</span><span class="sxs-lookup"><span data-stu-id="7797a-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>
  
<span data-ttu-id="7797a-110">เมื่อต้องการเพิ่มพื้นที่จัดเก็บข้อมูลของคุณใน OneDrive for Business ให้เลือกการสมัครใช้งานที่มี**onedrive For Business Plan 2**หรือ**Office ๓๖๕ E3**</span><span class="sxs-lookup"><span data-stu-id="7797a-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 E3**.</span></span>
  
<span data-ttu-id="7797a-111">เมื่อต้องการเปลี่ยนแผนในศูนย์การจัดการให้ไปที่หน้าการ**เรียกเก็บเงิน** \> [ของผลิตภัณฑ์ของคุณ](https://go.microsoft.com/fwlink/p/?linkid=842054)เลือกการสมัครใช้งานเพื่อเปลี่ยนจากนั้นเลือก**ดูการอัปเกรดที่แนะนำสำหรับองค์กรของคุณ**</span><span class="sxs-lookup"><span data-stu-id="7797a-111">To change plans, in the admin center, go to the **Billing** \> [Your products](https://go.microsoft.com/fwlink/p/?linkid=842054) page, select the subscription to change, then choose **View upgrades recommended for your org**.</span></span>
  
<span data-ttu-id="7797a-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงแผนและที่เก็บข้อมูล OneDrive for Business ให้ดู[อัปเกรดเป็นแผนอื่น](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)และ[คำอธิบายบริการ OneDrive for Business](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)</span><span class="sxs-lookup"><span data-stu-id="7797a-112">For more information on changing plans and OneDrive for Business storage, see [Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) and the [OneDrive for Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>