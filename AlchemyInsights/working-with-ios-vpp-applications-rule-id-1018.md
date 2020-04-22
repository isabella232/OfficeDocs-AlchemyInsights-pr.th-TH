---
title: การทํางานกับ iOS VPP แอพลิเคชันกฎ ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719976"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="94398-102">การทํางานกับแอปพลิเคชัน iOS VPP</span><span class="sxs-lookup"><span data-stu-id="94398-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="94398-103">[อ่านวิธีจัดการแอป iOS ที่ซื้อผ่านโปรแกรมการซื้อแบบจํานวนมากด้วย Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios)เพื่อเรียนรู้เกี่ยวกับคุณลักษณะ ข้อจํากัด และขั้นตอนต่างๆ ในการใช้โปรแกรมการซื้อไดรฟ์ข้อมูล Apple และการสนับสนุนสําหรับแอปใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="94398-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="94398-104">**ปัญหาที่พบบ่อย:** "ฉันกําหนดแอป iOS VPP ให้กับผู้ใช้ของฉัน แต่การติดตั้งล้มเหลว"</span><span class="sxs-lookup"><span data-stu-id="94398-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="94398-105">กรณีนี้สามารถเกิดขึ้นได้หากมีการใช้โทเค็น VPP เพียงโทเค็นเดียวในผู้ให้บริการการจัดการอุปกรณ์เคลื่อนที่หลายราย</span><span class="sxs-lookup"><span data-stu-id="94398-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="94398-106">สัญญาณ VPP จาก Apple สามารถใช้กับผู้ให้บริการรายเดียวเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="94398-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="94398-107">ถ้าคุณใช้โทเค็น VPP กับผู้ให้บริการหลาย คุณต้องอัปโหลดโทเค็นอีกครั้งเพื่อ Intune</span><span class="sxs-lookup"><span data-stu-id="94398-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="94398-108">การติดตั้งยังสามารถล้มเหลวถ้าจํานวนการติดตั้งทั้งหมดเกินจํานวนสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="94398-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="94398-109">เมื่อต้องการดูรายงานการใช้งานสําหรับสิทธิ์การใช้งานของคุณ ให้ไปที่หน้า**สิทธิ์การใช้งานแอป** **Intune Mobile App** \></span><span class="sxs-lookup"><span data-stu-id="94398-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="94398-110">เมื่อต้องการเรียนรู้วิธีการเรียกคืนสิทธิ์การใช้งานที่ใช้ โปรดดูที่[บทความนี้](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="94398-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
