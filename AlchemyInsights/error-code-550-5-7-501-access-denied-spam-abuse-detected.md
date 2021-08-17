---
title: รหัสข้อผิดพลาด 550 5.7.501 การเข้าถึงถูกปฏิเสธ พบการสแปม
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
ms.openlocfilehash: a3eebe4e9d69e100a750e74a6d34ec67dc0566df5dd6eb59809adb07ed8a682f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044287"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 การเข้าถึงถูกปฏิเสธ พบการสแปม

โดยทั่วไป ข้อความนี้จะเกิดขึ้นเมื่อผู้ใช้ส่งข้อความอีเมลจากที่อยู่ IP โดยใช้โดเมน *.onmicrosoft.com* เริ่มต้นที่มอบหมายให้กับผู้เช่าใหม่ใน Microsoft 365 วิธีที่ง่ายที่สุดในการแก้ไขปัญหานี้คือ:

1. [เพิ่มโดเมนลงในผู้เช่า](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)ของคุณ

2. [เปลี่ยนที่อยู่อีเมลหลักของผู้ใช้เป็นโดเมน](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) แบบปรับแต่งเองใหม่ที่คุณเพิ่งเพิ่ม
