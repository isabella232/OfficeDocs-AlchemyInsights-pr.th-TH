---
title: ข้อคิดเห็นเกี่ยวกับรายการ
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724173"
---
# <a name="comments-on-list-items"></a>ข้อคิดเห็นเกี่ยวกับรายการ

ผู้ใช้สามารถดูข้อคิดเห็นทั้งหมดในตัวเลือกรายการและกรองระหว่างมุมมองที่แสดงข้อคิดเห็นหรือกิจกรรมที่เกี่ยวข้องกับรายการได้

ผู้ใช้จำเป็นต้องบันทึกสิ่งต่อไปนี้ก่อนที่พวกเขาจะสามารถเพิ่มและลบข้อคิดเห็น:

- ข้อคิดเห็นให้ทำตามการตั้งค่าสิทธิ์โดยธรรมชาติใน SharePoint
- รายการคลาสสิกที่ยังไม่ได้สร้างขึ้นเพื่อแสดงในส่วนติดต่อผู้ใช้ที่ทันสมัยเช่นรายการงานจะไม่มีฟีเจอร์การแสดงข้อคิดเห็นนี้
- การแสดงความคิดเห็นเกี่ยวกับรายการในทีมไม่พร้อมใช้งานกับรุ่นนี้
- ข้อคิดเห็นไม่ได้รับการทำดัชนีด้วยการค้นหา

ผู้ดูแลระบบสามารถปิดใช้งานฟีเจอร์นี้ได้ที่ระดับองค์กรโดยการเปลี่ยนพารามิเตอร์ **CommentsOnListItemsDisabled** ใน Cmdlet การ **ตั้งค่า-SPOTenant** PowerShell

ในตอนนี้ยังไม่สามารถปิดใช้งานการแสดงข้อคิดเห็นที่ไซต์หรือระดับรายการได้ เราหวังว่าจะมีตัวควบคุมเหล่านี้ในการอัปเดตในภายหลังซึ่งมีแนวโน้มในไตรมาสแรก๒๐๒๑
