---
title: สิทธิ์และความยินยอมของ API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974996"
---
# <a name="api-permissions-and-consent"></a>สิทธิ์และความยินยอมของ API

แอปพลิเคชันที่รวมเข้ากับ Microsoft identity platform จะทำตามรูปแบบการตรวจสอบที่ทำให้ผู้ใช้และผู้ดูแลระบบสามารถควบคุมได้ว่าจะสามารถเข้าถึงข้อมูลได้อย่างไร การใช้งานของแบบจำลองการตรวจสอบได้รับการอัปเดตในจุดสิ้นสุดของแพลตฟอร์มสำหรับข้อมูลประจำตัวของ Microsoft การเปลี่ยนแปลงวิธีที่แอปจะต้องโต้ตอบกับแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft [สิทธิ์และความยินยอมในจุดสิ้นสุดของแพลตฟอร์มสำหรับข้อมูลประจำ](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) ตัวของ Microsoft ครอบคลุมแนวคิดพื้นฐานของรูปแบบการตรวจสอบนี้รวมถึงขอบเขตสิทธิ์และความยินยอม

[กรอบความยินยอมของ Azure Active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework)ทำให้ง่ายต่อการพัฒนาเว็บไซต์ผู้เช่าหลายรายและแอปพลิเคชันไคลเอ็นต์ดั้งเดิม แอปพลิเคชันเหล่านี้อนุญาตให้เข้าสู่ระบบโดยบัญชีผู้ใช้จากผู้เช่าโฆษณา Azure ที่แตกต่างจากที่มีการลงทะเบียนแอปพลิเคชัน นอกจากนี้พวกเขาอาจจำเป็นต้องเข้าถึงเว็บ APIs เช่น Microsoft Graph API (ในการเข้าถึง Azure AD, Intune และบริการใน Microsoft ๓๖๕) และอื่นๆของ Microsoft services APIs นอกเหนือจากเว็บ APIs ของคุณเอง

