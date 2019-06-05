---
title: สร้าง และใช้กล่องจดหมายที่ใช้ร่วมกัน
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717365"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>แก้ไขปัญหา - ไม่พบในไดเรกทอรีของผู้ใช้

<p>ถ้าผู้ใช้ได้รับข้อความแสดงข้อผิดพลาด<strong> &ldquo;&hellip;ผู้ใช้สามารถ&rsquo;t พบในไดเรกทอรีได้ โปรดลองอีกครั้ง&hellip;</strong>ซึ่งเป็นชนิดการตัดสินค้าจากคลัง<strong>&ldquo;ผู้ใช้ที่ไม่ได้อยู่ในไดเรกทอรีได้&rdquo;</strong>จะเสร็จขั้นตอนต่อไปนี้เพื่อแก้ไขปัญหานี้ได้</p> <ol> <li>ให้แน่ใจว่าบัญชีที่ยอมรับการเชิญทางอีเมลเป็นบัญชีเดียวกับที่ใช้เข้าสู่ระบบในภายหลัง ตรวจสอบให้แน่ใจว่า ผู้ใช้ที่กำลังใช้บัญชีเดียวกันเพื่อยอมรับการเชิญ และเซ็นชื่อลงในไซต์ <br /><br />สำหรับข้อมูลเพิ่มเติม ให้ดู<a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">วิธีการจัดการนามแฝงสำหรับบัญชี Microsoft ของคุณ</a>ในการจัดการการเข้าสู่ระบบ Office 365 <br /><br /></li> <li>เรียกดูไซต์แต่ละผู้ใช้ได้รับข้อผิดพลาด <br /><br />อยู่ เพิ่ม<strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (ภายในอัญประกาศ) ลงในส่วนท้ายของ URL ของไซต์ <br /><br />ตัวอย่าง: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b เลือกผู้ใช้จากรายการ <br /><br />c คลิก<strong>เอาออกสิทธิ์ของผู้ใช้จาก Ribbon</strong> <br /><br />d เพิ่มผู้ใช้กลับ และส่งการเชิญไปยังผู้ใช้</li> </ol>

