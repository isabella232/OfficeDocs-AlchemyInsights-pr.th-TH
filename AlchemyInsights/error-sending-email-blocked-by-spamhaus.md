---
title: เกิดข้อผิดพลาดในการส่งอีเมลที่ถูกบล็อกโดย SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813743"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>ข้อผิดพลาดในการส่งอีเมล: โฮสต์ไคลเอ็นต์ถูกบล็อกโดยใช้ Spamhaus

ที่อยู่ IP ที่ส่งข้อความอยู่ในรายการบล็อกที่เป็นของ[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245) เหตุผลที่ถูกบล็อกโดย Spamhaus รวมถึงบัญชีที่ถูกละเมิด การใช้งานเครื่องที่ถูกละเมิดการแชร์ที่อยู่ IP สาธารณะ และนโยบายของผู้ให้บริการอินเทอร์เน็ต (ISP) การแก้ไขที่เป็นไปได้คือ:
  
- For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.

- For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. ถ้าที่อยู่ IP อยู่ในรายการบล็อกนโยบาย (PBL) เจ้าของสามารถกําหนดที่อยู่ IP แบบคงที่อื่น หรือเอาที่อยู่ออกจาก PBL ได้

- For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service. คุณสามารถใช้เครื่องมือการค้นหา WHOIS เพื่อค้นหาเจ้าของที่อยู่ IP ที่ถูกบล็อก
