---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713665"
---
# <a name="move-email-to-the-archive-mailbox"></a>ย้ายอีเมลไปยังกล่องจดหมายเก็บถาวร

1. ยืนยันว่า**กล่องจดหมายเก็บถาวร**ถูกเปิดใช้งาน ถ้าไม่ ใช้ขั้นตอน[ในบทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)เพื่อเปิดใช้งานกล่องจดหมายเก็บถาวร

2. หากต้องการเก็บถาวรข้อความโดยอัตโนมัติไปยังกล่องจดหมายเก็บถาวร**Move to archive****applied automatically to entire mailbox (default) tag** ใช้ขั้นตอนที่นี่เพื่อสร้างแท็ก:[แท็กเริ่มต้นเก็บถาวร](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. จากนั้นให้เพิ่มแท็ก**เก็บถาวร**ในนโยบายการเก็บข้อมูล ในศูนย์การจัดการ Exchange ให้เลือก**นโยบายการเก็บข้อมูล**>เพิ่ม **>****แท็ก**

4. ตอนนี้[กําหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)ไปยังกล่องจดหมายของผู้ใช้ที่ระบุ นโยบายเดียวกันจะนําไปใช้กับทั้ง**หลัก**และกล่องจดหมาย**การเก็บถาวร**

คุณอาจจําเป็นต้องบังคับให้มีการจัดการโฟลเดอร์ผู้ช่วย (MFA) เพื่อเรียกใช้ และใช้การตั้งค่าใหม่ไปยังกล่องจดหมายของผู้ใช้ เรียกใช้คําสั่งต่อไปนี้ขณะเชื่อมต่อกับ[PowerShell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นตัวจัดการโฟลเดอร์ช่วยสําหรับกล่องจดหมายที่ระบุ:
  
เริ่มต้นจัดการโฟลเดอร์ผู้ช่วย -ข้อมูลเฉพาะตัว<name of the mailbox>

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวร ให้ดูที่[การตั้งค่านโยบายการเก็บถาวรและการลบสําหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  