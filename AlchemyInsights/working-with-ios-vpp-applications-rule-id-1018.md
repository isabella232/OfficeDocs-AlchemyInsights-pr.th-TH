---
title: การทำงานกับ iOS VPP 1018 Id กฎของแอพลิเคชัน
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917515"
---
# <a name="working-with-ios-vpp-applications"></a>การทำงานกับโปรแกรมประยุกต์ VPP iOS

อ่าน[วิธีการจัดการโปรแกรมประยุกต์ iOS ซื้อผ่านโปรแกรม volume ซื้อกับ Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios)เพื่อเรียนรู้เกี่ยวกับคุณลักษณะ ข้อจำกัด และขั้นตอนการทำให้ใช้ของ Apple ปริมาตรซื้อโปรแกรมและการสนับสนุนสำหรับตารางนั้นใน Microsoft Intune 
  
 **ปัญหา:** "ฉันได้กำหนดแอพลิเคชัน VPP iOS ผู้ใช้ของฉัน แต่การติดตั้งล้มเหลว" 
  
- ซึ่งสามารถเกิดขึ้นได้ถ้ามีใช้โทเค็น VPP เดียวระหว่างผู้ให้บริการการจัดการอุปกรณ์เคลื่อนที่หลาย ๆ โทเค็น VPP จากเครื่องคอมพิวเตอร์ Apple อาจใช้ได้กับผู้ให้บริการหนึ่งเท่านั้น ถ้าคุณใช้โทเค็น VPP กับผู้ให้บริการหลาย คุณต้องอัปโหลดโทเค็นการ Intune อีกครั้ง
    
- การติดตั้งสามารถล้มเหลวได้นอกจากนี้ถ้าจำนวนทั้งหมดที่ติดตั้งเกินจำนวนของสิทธิ์การใช้งาน เมื่อต้องการดูรายงานการใช้งานสำหรับสิทธิ์การใช้งานของคุณ ไปที่**apps Intune Mobile** \>เพจ**สิทธิ์การใช้งานโปรแกรมประยุกต์** เมื่อต้องการเรียนรู้วิธีการเพิ่มสิทธิ์การใช้งานใช้ ดู[บทความนี้](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

