---
title: ข้อคิดเห็นบนข้อมูลในรายการ
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
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995526"
---
# <a name="comments-on-list-items"></a>ข้อคิดเห็นบนข้อมูลในรายการ

ผู้ใช้สามารถดูข้อคิดเห็นทั้งหมดบนข้อมูลในรายการและตัวกรองระหว่างมุมมองที่แสดงข้อคิดเห็นหรือกิจกรรมที่เกี่ยวข้องกับข้อมูลได้

ผู้ใช้ต้องจดบันทึกสิ่งต่อไปนี้ก่อน จึงจะสามารถเพิ่มและลบข้อคิดเห็นได้:

- ข้อคิดเห็นจะเป็นไปตามการตั้งค่าสิทธิ์SharePointโฟลเดอร์
- รายการแบบคลาสสิกที่ยังไม่ได้สร้างขึ้นเพื่อแสดงในส่วนติดต่อผู้ใช้ที่ทันสมัย เช่น รายการงาน จะยังไม่มีฟีเจอร์การแสดงข้อคิดเห็นนี้
- ข้อคิดเห็นบนรายการTeamsไม่พร้อมใช้งานกับรุ่นนี้
- ข้อคิดเห็นจะไม่ถูกสร้างดัชนีโดยการค้นหา

ผู้ดูแลระบบสามารถปิดใช้งานฟีเจอร์นี้ที่ระดับองค์กรโดยการเปลี่ยนพารามิเตอร์ **CommentsOnListItemsDisabled** ใน **cmdlet Set-SPOTenant** PowerShell

ขณะนี้ยังไม่สามารถปิดใช้งานการแสดงข้อคิดเห็นที่ระดับไซต์หรือรายการได้ เราหวังว่าจะมีตัวควบคุมเหล่านั้นในการอัปเดตในภายหลัง ในไตรมาสแรกปี 2021
