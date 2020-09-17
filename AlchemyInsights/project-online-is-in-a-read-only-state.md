---
title: Project Online อยู่ในสถานะแบบอ่านอย่างเดียว
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801671"
---
# <a name="project-online-is-in-a-read-only-state"></a>Project Online อยู่ในสถานะแบบอ่านอย่างเดียว

มีสาเหตุทั่วไปสามประการที่ทำให้ Project Online สามารถเข้าถึงสถานะแบบอ่านอย่างเดียวได้:

1. องค์กรมีการให้สิทธิ์การใช้งานสิ่งจำเป็นสำหรับ Project Online เท่านั้น นี่ไม่เพียงพอที่จะทำให้ไซต์มีชีวิตอยู่และในที่สุดจะได้รับการเตรียมใช้งานเราวางไซต์ในสถานะแบบอ่านอย่างเดียวเพื่อให้ผู้ดูแลระบบทราบว่ามีบางสิ่งผิดปกติและสามารถรับสิทธิ์การใช้งานที่ถูกต้องได้ ผู้ดูแลระบบจะต้องเพิ่มสิทธิ์การใช้งาน Project Online และ/หรือสิทธิ์การใช้งานพิเศษ ไซต์จะออกจากแบบอ่านอย่างเดียวที่จุดนั้น สำหรับข้อมูลเพิ่มเติมให้ดูที่[เปรียบเทียบโซลูชันการจัดการโครงการ](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)
2. มีการเข้าถึงโควตาที่ได้รับมอบหมายแล้ว สำหรับข้อมูลเพิ่มเติมให้ดูที่[โควตาของ Project Web App](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota) ตรวจสอบการ [กำหนดค่าสะสมของข้อมูลการรายงานจเข้าใน Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) เพื่อดูว่าองค์ประกอบของรายงานอาจส่งผลกระทบต่อการใช้งานโควตาอย่างไร
3. แบบอ่านอย่างเดียวอาจเป็นเงื่อนไขชั่วคราวที่อาจเกิดขึ้นในระหว่างการบำรุงรักษา การบำรุงรักษาส่วนใหญ่จะไม่ได้รับการสังเกตเห็นโดยลูกค้าของเราและคุณจะไม่เห็นสิ่งนี้แต่จะมีบางครั้งที่มีการใช้งานแบบอ่านอย่างเดียวในช่วงเวลาสั้นๆ
