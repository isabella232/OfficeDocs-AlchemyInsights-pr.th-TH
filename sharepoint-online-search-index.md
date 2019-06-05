---
title: จัดการการค้นหาพจนานุกรมใน SharePoint แบบออนไลน์
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 4b51c6d44940c1a65ecf93a149430f05882452ba
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715370"
---
# <a name="search-in-sharepoint-online"></a>ค้นหาใน SharePoint แบบออนไลน์

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin; color: black; background: white;">เนื้อหาต้องตระเวน และเพิ่มลงในดัชนีการค้นหาสำหรับผู้ใช้ในการค้นหาสิ่งที่กำลังค้นหาใน SharePoint แบบออนไลน์ เนื้อหาถูกตระเวนโดยอัตโนมัติตามตารางเวลาการตระเวนที่กำหนดไว้ล่วงหน้า (ไม่สามารถเปลี่ยนแปลงตารางเวลาการตระเวน) ตัวตระเวนรับค่าเนื้อหาที่มีการเปลี่ยนแปลงนับตั้งแต่การตระเวนครั้งล่าสุด และการปรับปรุงดัชนี</span> เพื่อให้แน่ใจว่า ตระเวนเนื้อหา และมีการปรับปรุงดัชนี ทำตามขั้นตอนด้านล่างนี้</p> <ol style="margin-top: 0in;" start="1" type="1"> <li style="color: black; ; font-size: 11pt; font-style: normal; font-weight: 400; margin-left: 0in;"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin; background: white;">ตรวจสอบให้แน่ใจว่า เนื้อหาสามารถค้นพบได้ โดยการทำให้สามารถค้นหาเนื้อหาไซต์ สำหรับข้อมูลเพิ่มเติม ดู<a href="https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable">เปิดเนื้อหาบนไซต์ให้สามารถค้นหาได้</a> <br /><br /></span></li> <li style="color: black; ; font-size: 11pt; font-style: normal; font-weight: 400; margin-left: 0in;"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin; background: white;"><span style="display: inline !important; float: none; background-color: #ffffff; color: #000000; font-family: Segoe UI,SegoeUI,Segoe WP,Helvetica Neue,Helvetica,Tahoma,Arial,sans-serif; font-size: 16px; font-style: normal; font-variant: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: left; text-decoration: none; text-indent: 0px; text-transform: none; -webkit-text-stroke-width: 0px; white-space: normal; word-spacing: 0px;">เมื่อคุณเปลี่ยนแปลงคุณสมบัติที่มีการจัดการ หรือ เมื่อคุณได้เปลี่ยนการแมปคุณสมบัติที่ตระเวน และที่มีการจัดการ<strong>ไซต์จะถูกตระเวนใหม่</strong>ก่อนการเปลี่ยนแปลงของคุณจะมีผลต่อดัชนีการค้นหาด้วย <span style="display: inline !important; float: none; background-color: #ffffff; color: #000000; font-family: Segoe UI,SegoeUI,Segoe WP,Helvetica Neue,Helvetica,Tahoma,Arial,sans-serif; font-size: 16px; font-style: normal; font-variant: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: left; text-decoration: none; text-indent: 0px; text-transform: none; -webkit-text-stroke-width: 0px; white-space: normal; word-spacing: 0px;">ได้เนื่องจากมีทำการเปลี่ยนแปลงของคุณใน schema ค้นหา และไม่ให้ไซต์จริง ตัวตระเวนจะไม่อัตโนมัติใหม่ดัชนีให้กับไซต์</span></span> </span> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin; color: windowtext;">สำหรับข้อมูลเพิ่มเติม ดู<a href="https://docs.microsoft.com/en-us/sharepoint/crawl-site-content">ขอตระเวน และการทำดัชนีของไซต์ ไลบรารีหรือรายการใหม่ด้วยตนเอง</a>&nbsp;<br /><br /></span><strong style="mso-bidi-font-weight: normal;"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">หมายเหตุ:</span> </strong> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">รออย่างน้อย 24 ชั่วโมงหลังจากการร้องขอการตระเวนและแบบเต็มดัชนีใหม่เมื่อต้องการดูถ้าคุณยังคงประสบกับปัญหาด้วยตนเอง <span style="color: black; background: white;">ถ้ามากกว่า 24 ชั่วโมงได้ตั้งแต่เริ่มต้นการตระเวนและเต็มจัดดัชนี โปรดเข้าสู่ระบบสนับสนุนกรณีและปัญหา ในหลายกรณี เรากำลังทำงานอยู่ในโซลูชัน โปรดให้กับเราอย่างน้อย 24 ชั่วโมงในการแก้ไขปัญหาการทำให้เสร็จสมบูรณ์<br /><br /></span></span><strong style="mso-bidi-font-weight: normal;"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">สำคัญ:</span></strong> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ถ้าไซต์ เอกสาร (ไลบรารี), หรือรายการถูกลบ และยังคง แสดงให้เห็นในผลลัพธ์การค้นหา ผู้ใช้ควรได้รับข้อผิดพลาด 404 ไม่พบแฟ้มเมื่อพยายามเข้าถึง ปัญหานี้ควรเข้าสู่ระบบเป็นกรณีและปัญหาสนับสนุนสำหรับการสืบสวนเพิ่มเติม </span></li> </ol>



