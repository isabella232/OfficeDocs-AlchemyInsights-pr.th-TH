---
title: การทำงานกับ iOS VPP 1018 Id กฎของแอพลิเคชัน
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28317095"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="c3bfe-102">การทำงานกับโปรแกรมประยุกต์ VPP iOS</span><span class="sxs-lookup"><span data-stu-id="c3bfe-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="c3bfe-103">อ่าน[วิธีการจัดการโปรแกรมประยุกต์ iOS ซื้อผ่านโปรแกรม volume ซื้อกับ Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios)เพื่อเรียนรู้เกี่ยวกับคุณลักษณะ ข้อจำกัด และขั้นตอนการทำให้ใช้ของ Apple ปริมาตรซื้อโปรแกรมและการสนับสนุนสำหรับตารางนั้นใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c3bfe-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="c3bfe-104">**ปัญหา:** "ฉันได้กำหนดแอพลิเคชัน VPP iOS ผู้ใช้ของฉัน แต่การติดตั้งล้มเหลว"</span><span class="sxs-lookup"><span data-stu-id="c3bfe-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="c3bfe-p101">ซึ่งสามารถเกิดขึ้นได้ถ้ามีใช้โทเค็น VPP เดียวระหว่างผู้ให้บริการการจัดการอุปกรณ์เคลื่อนที่หลาย ๆ โทเค็น VPP จากเครื่องคอมพิวเตอร์ Apple อาจใช้ได้กับผู้ให้บริการหนึ่งเท่านั้น ถ้าคุณใช้โทเค็น VPP กับผู้ให้บริการหลาย คุณต้องอัปโหลดโทเค็นการ Intune อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="c3bfe-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="c3bfe-p102">การติดตั้งสามารถล้มเหลวได้นอกจากนี้ถ้าจำนวนทั้งหมดที่ติดตั้งเกินจำนวนของสิทธิ์การใช้งาน เมื่อต้องการดูรายงานการใช้งานสำหรับสิทธิ์การใช้งานของคุณ ไปที่**apps Intune Mobile** \>เพจ**สิทธิ์การใช้งานโปรแกรมประยุกต์** เมื่อต้องการเรียนรู้วิธีการเพิ่มสิทธิ์การใช้งานใช้ ดู[บทความนี้](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="c3bfe-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

