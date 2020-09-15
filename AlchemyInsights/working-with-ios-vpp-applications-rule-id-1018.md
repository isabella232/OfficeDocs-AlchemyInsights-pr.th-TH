---
title: การทำงานกับ iOS VPP Id กฎของแอปพลิเคชัน๑๐๑๘
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688965"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="e6f4b-102">การทำงานกับแอปพลิเคชัน iOS VPP</span><span class="sxs-lookup"><span data-stu-id="e6f4b-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="e6f4b-103">อ่าน [วิธีการจัดการแอป iOS ที่ซื้อผ่านโปรแกรมการสั่งซื้อโดยใช้ระดับเสียงด้วย Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) เพื่อเรียนรู้เกี่ยวกับฟีเจอร์ข้อจำกัดและขั้นตอนในการใช้โปรแกรมการซื้อปริมาณของ Apple และการสนับสนุนใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e6f4b-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="e6f4b-104">**ปัญหาทั่วไป:** "ฉันได้กำหนดแอป iOS VPP ให้กับผู้ใช้ของฉันแต่การติดตั้งล้มเหลว"</span><span class="sxs-lookup"><span data-stu-id="e6f4b-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="e6f4b-105">กรณีนี้อาจเกิดขึ้นได้ถ้ามีการใช้โทเค็น VPP หนึ่งตัวในผู้ให้บริการการจัดการอุปกรณ์เคลื่อนที่หลายรายการ</span><span class="sxs-lookup"><span data-stu-id="e6f4b-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="e6f4b-106">โทเค็น VPP จาก Apple อาจใช้กับผู้ให้บริการหนึ่งคนเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="e6f4b-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="e6f4b-107">ถ้าคุณใช้โทเค็น VPP กับผู้ให้บริการหลายรายคุณจะต้องอัปโหลดโทเค็นไปยัง Intune อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="e6f4b-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="e6f4b-108">การติดตั้งยังอาจล้มเหลวถ้าจำนวนการติดตั้งทั้งหมดเกินจำนวนสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e6f4b-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="e6f4b-109">เมื่อต้องการดูรายงานการใช้งานสำหรับสิทธิ์การใช้งานของคุณให้ไปที่หน้าสิทธิ์การใช้งานแอ**ปสำหรับอุปกรณ์เคลื่อนที่ของ Intune** \> **App licenses**</span><span class="sxs-lookup"><span data-stu-id="e6f4b-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="e6f4b-110">เมื่อต้องการเรียนรู้วิธีการเพิ่มสิทธิ์การใช้งานให้ดู [บทความนี้](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="e6f4b-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
