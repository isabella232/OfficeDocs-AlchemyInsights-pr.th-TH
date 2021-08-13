---
title: การเปลี่ยนสิทธิ์ของโฟลเดอร์สาธารณะ
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: 16c2fb89f8dd256afb7e922ca74976097501173bf605e6c5fccc73019a71edcd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950207"
---
# <a name="changing-public-folder-permissions"></a>การเปลี่ยนสิทธิ์ของโฟลเดอร์สาธารณะ

สิทธิ์ของโฟลเดอร์สาธารณะสามารถเปลี่ยนแปลงได้โดยผู้ใช้และผู้ดูแลระบบOutlookโฟลเดอร์ ผู้ดูแลระบบยังสามารถควบคุมสิทธิ์จากศูนย์Exchangeการจัดการระบบ (EAC) ได้โดยเลือกดังต่อไปนี้
  
1. ในศูนย์การจัดการ Microsoft 365 ให้ไปที่ **ศูนย์การจัดการ** \> **Exchange**

2. เลือก **โฟลเดอร์** สาธารณะ

3. จากที่นั่น คุณสามารถเปลี่ยนสิทธิ์ของโฟลเดอร์สาธารณะแต่ละโฟลเดอร์ได้โดยการกําหนดกลุ่มความปลอดภัยให้กับสิทธิ์ เพื่อให้ผู้ใช้เปลี่ยนสิทธิ์ของโฟลเดอร์สาธารณะ ผู้ใช้ต้องมีสิทธิ์ เจ้าของ ในโฟลเดอร์

โปรดปฏิบัติตามขั้นตอนที่อธิบายไว้ใน [วิธีวินิจฉัยและแก้ไขปัญหาสิทธิ์ในการเข้าถึงโฟลเดอร์](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) สาธารณะเพื่อแก้ไขปัญหาสิทธิ์ของโฟลเดอร์สาธารณะ

**หมายเหตุ**: มีปัญหาที่ทราบแล้วมากมายที่คุณอาจพบเมื่อคุณพยายามเปลี่ยนสิทธิ์ในโฟลเดอร์สาธารณะ ดูบทความต่อไปนี้เพื่อดูข้อมูลเพิ่มเติม

- [ไม่สามารถใช้สิทธิ์กับโฟลเดอร์ย่อยสาธารณะใน EAC ได้](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [ข้อผิดพลาด "ไม่พบกล่องจดหมายในฟอเรสต์ภายใน" เมื่อคุณเข้าถึงโฟลเดอร์สาธารณะ](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
