---
title: สิทธิ์และการยินยอมของ API
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932116"
---
# <a name="api-permissions-and-consent"></a>สิทธิ์และความยินยอมของ API

แอปพลิเคชันที่รวมแพลตฟอร์มข้อมูลประจําตัวของ Microsoftติดตามรูปแบบการอนุญาตที่ให้ผู้ใช้และผู้ดูแลระบบควบคุมวิธีเข้าถึงข้อมูล การปรับใช้รูปแบบการอนุญาตได้รับการอัปเดตบนแพลตฟอร์มข้อมูลประจําตัวของ Microsoftสิ้นสุด แอปจะเปลี่ยนวิธีที่แอปต้องโต้ตอบกับแพลตฟอร์มข้อมูลประจําตัวของ Microsoftของคุณ [สิทธิ์และความยินยอมในแพลตฟอร์มข้อมูลประจําตัวของ Microsoftปลายทาง](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)จะครอบคลุมแนวคิดพื้นฐานของรูปแบบการอนุญาตนี้ รวมถึงขอบเขต สิทธิ์ และความยินยอม

เฟรม[Azure Active Directoryการยินยอมแบบหลายผู้เช่า (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework)จะเป็นเรื่องง่ายที่จะพัฒนาเว็บหลายผู้เช่าและแอปพลิเคชันไคลเอ็นต์ดั้งเดิม แอปพลิเคชันเหล่านี้อนุญาตให้ลงชื่อเข้าใช้ด้วยบัญชีผู้ใช้จากผู้เช่า Azure AD ที่แตกต่างจากที่ลงทะเบียนแอปพลิเคชัน พวกเขาอาจยังต้องเข้าถึง API ของเว็บ เช่น Microsoft Graph API (เพื่อเข้าถึง Azure AD, Intuned และบริการใน Microsoft 365) และ API ของ บริการของ Microsoft อื่นๆ นอกเหนือจาก API เว็บของคุณเอง

