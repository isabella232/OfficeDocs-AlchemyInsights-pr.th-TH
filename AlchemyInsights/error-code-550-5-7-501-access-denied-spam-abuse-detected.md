---
title: รหัสข้อผิดพลาด๕๕๐การเข้าถึง5.7.501 ถูกปฏิเสธการตรวจพบการละเมิดของสแปม
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784074"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>๕๕๐ 5.7.501 Access ถูกปฏิเสธการตรวจพบการละเมิดสแปม

โดยทั่วไปแล้วข้อความนี้จะเกิดขึ้นเมื่อผู้ใช้ส่งข้อความอีเมลจากที่อยู่ IP โดยใช้โดเมน *onmicrosoft.com ที่ได้* รับมอบหมายให้กับผู้เช่าใหม่ใน Microsoft ๓๖๕ วิธีที่ง่ายที่สุดในการแก้ไขปัญหานี้คือ:

1. [เพิ่มโดเมนลงในผู้เช่าของคุณ](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)

2. [เปลี่ยนที่อยู่อีเมลหลักของผู้ใช้ของคุณ](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) ไปเป็นโดเมนแบบกำหนดเองใหม่ที่คุณเพิ่งเพิ่มเข้าไป
