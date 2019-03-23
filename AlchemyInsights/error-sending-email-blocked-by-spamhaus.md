---
title: ข้อผิดพลาดในการส่งอีเมลที่ถูกบล็อก โดย SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2019
ms.locfileid: "30761652"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>ข้อผิดพลาดในการส่งอีเมล: โฮสต์ของไคลเอนต์ที่ถูกบล็อคโดยใช้ Spamhaus

อยู่ IP ที่ส่งข้อความในรายการบล็อก[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)เป็นเจ้าของอยู่ สาเหตุถูกบล็อคโดย Spamhaus รวมบัญชีถูกโจมตี โจมตีเครื่องที่ใช้ที่อยู่ IP สาธารณะ และนโยบายของผู้ให้บริการอินเทอร์เน็ต (ISP) ร่วมกัน การแก้ไขปัญหาที่เป็นไปได้คือ:
  
- หาถูกบล็อคขาเข้าถึง Office 365 ซึ่งคุณควบคุมเซิร์ฟเวอร์อีเมลแหล่งที่มา คุณจำเป็นต้องค้นหาสาเหตุ และบล็อคการเอาออกจากเว็บไซต์ Spamhaus
    
- หาถูกบล็อคขาเข้าไปที่ที่อยู่ IP ของแหล่งที่มาเป็นสมาชิกคนอื่นของ Office 365 เจ้าของที่อยู่ต้องเอาบล็อคจากเว็บไซต์ Spamhaus ถ้าอยู่ IP บนรายการบล็อกนโยบาย (PBL), เจ้าของสามารถกำหนดที่อยู่ IP แบบคงอื่น หรือเอาอยู่จาก PBL
    
- หาถูกบล็อคขาออกจากโดเมน Office 365 ของคุณ คุณสามารถได้รับข้อผิดพลาดนี้ถ้าข้อความถูกจัดเส้นทางผ่านฝ่ายบริการที่ 3 คุณสามารถใช้เครื่องมือค้นหา WHOIS เพื่อค้นหาเจ้าของที่อยู่ IP ที่ถูกบล็อค
    

