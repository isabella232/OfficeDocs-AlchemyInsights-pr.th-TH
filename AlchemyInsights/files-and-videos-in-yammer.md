---
title: ไฟล์และวิดีโอใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6040"
- "9003112"
ms.openlocfilehash: c5f2b7f6ac4686bc9ef81c38525994d032a57f78
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745221"
---
# <a name="files-and-videos-in-yammer"></a>ไฟล์และวิดีโอใน Yammer

สามารถแนบไฟล์กับข้อความใน Yammer หรืออัปโหลดไปยังกลุ่มได้โดยตรง ประสบการณ์การใช้งานของผู้ใช้จะแตกต่างกันเล็กน้อยระหว่าง Yammer แบบคลาสสิกและใหม่แต่ไฟล์จะถูกอัปโหลดไปยังตำแหน่งที่ตั้งเดียวกัน สำหรับข้อมูลเพิ่มเติมให้ดู[ที่แนบไฟล์หรือรูปภาพไปยังข้อความ Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)  

เมื่อผู้ใช้ประสบปัญหาให้ลองอัปโหลดจากเบราว์เซอร์หรืออุปกรณ์อื่น ใช้การเชื่อมต่อเครือข่ายที่เร็วที่สุดและเบราว์เซอร์ล่าสุดที่พร้อมใช้งาน การใช้หน้าต่างเบราว์เซอร์ใหม่เพื่อลงชื่อเข้าใช้อีกครั้งสามารถช่วยตรวจสอบให้แน่ใจว่าโทเค็น AD Azure ที่ถูกต้องจะพร้อมใช้งาน

การอัปโหลดวิดีโอไปยัง Yammer จำเป็นต้องมีการอัปโหลดและการเข้ารหัส สำหรับข้อมูลเพิ่มเติมให้ดู [ที่โพสต์วิดีโอใน Yammer อัปโหลดและเข้ารหัสแยกจาก](https://support.microsoft.com/office/video-posts-in-yammer-upload-and-encode-separately-5b3a348e-3a0a-4c4b-95b1-eabdf245ba25)กัน การเข้ารหัสอาจใช้เวลาในการทำให้เสร็จสมบูรณ์ทั้งนี้ขึ้นอยู่กับขนาดของวิดีโอ พิจารณาใช้ [Microsoft Stream](https://docs.microsoft.com/stream/overview) เพื่ออัปโหลดวิดีโอที่คุณกำลังแชร์ใน microsoft ๓๖๕

**การจำกัดการอัปโหลดไฟล์และรูปภาพ**

Yammer อนุญาตให้มีการอัปโหลดชนิดไฟล์ทั้งหมดตามค่าเริ่มต้น ผู้ดูแลระบบสามารถเปลี่ยนแปลงการตั้งค่าเพื่อบล็อกการอัปโหลดไฟล์ไปยัง Yammer ได้ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จำกัดผู้ที่สามารถอัปโหลดไฟล์และจำกัดรูปแบบไฟล์](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-yammer#restrict-who-can-upload-files-and-limit-file-formats) การตั้งค่าที่เกี่ยวข้องจะพร้อมใช้งานสำหรับการจำกัด Gif ใน Yammer สำหรับข้อมูลเพิ่มเติมให้ดู[ที่อนุญาตให้มีการเพิ่มอายุการทำงานในข้อความ](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-yammer#allow-tenor-gifs-in-messages)

**ที่เก็บไฟล์ Yammer**

Yammer ถูกรวมเข้ากับ Microsoft ๓๖๕และใช้ SharePoint Online สำหรับการอัปโหลดไฟล์ สำหรับข้อมูลเพิ่มเติมให้ดูที่[ภาพรวมของที่เก็บข้อมูลไฟล์ Yammer](https://docs.microsoft.com/yammer/get-started-with-yammer/file-storage) 

สำหรับประสบการณ์การใช้งานที่ดีที่สุดในการโยกย้ายไฟล์ไปยัง SharePoint Online เราขอแนะนำให้คุณกำหนดค่าเครือข่าย Yammer ของคุณสำหรับโหมด Native สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ภาพรวมของโหมด Native](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode) 