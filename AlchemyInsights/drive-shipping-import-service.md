---
title: การจัดส่งไดรฟ์ในบริการMicrosoft 365นําเข้าของคุณ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 1f286896f80a6bbabd4810f10fb0b8284fd13aba
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58311382"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>การจัดส่งไดรฟ์ในบริการMicrosoft 365นําเข้าของคุณ

ใช้การจัดส่งไดรฟ์โดยการคัดลอก PSTs ลงในฮาร์ดไดรฟ์ แล้วส่งฮาร์ดไดรฟ์ไปยัง Microsoft

เมื่อต้องการเริ่มงาน:

1. In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.

1. เลือก **เลือกชนิดงาน** นําเข้า **แล้วเลือก** ถัดไป

1. เมื่อต้องการดูขั้นตอนต่างๆ ของตัวเลือกการนําเข้านี้ **ให้เลือก จัดส่งฮาร์ดไดรฟ์ไปยังหนึ่งในที่ตั้งทางกายภาพ** ของเรา

ต่อไปนี้คือสิ่งที่ควรทราบ:

- คุณต้องได้รับมอบหมายบทบาทนําเข้าและส่งออกกล่องจดหมายExchange Onlineนําเข้าไฟล์ PST Microsoft 365กล่องจดหมายของคุณ
ประสิทธิภาพการคํานวณอาจได้รับผลกระทบจาก PSTs ที่มีขนาดใหญ่กว่า 20 GB

- สนับสนุนเฉพาะไดรฟ์โซลิดสสเตต (SSD) ขนาด 2.5 นิ้ว หรือฮาร์ดไดรฟ์ภายในแบบ SATA II/III ขนาด 2.5 นิ้วหรือ 3.5 นิ้วเท่านั้น
ฮาร์ดไดรฟ์ที่มีไฟล์ PST ต้องถูกเข้ารหัสลับด้วย BitLocker

- ค่าใช้จ่ายในการนําเข้าไฟล์ PST Microsoft 365กล่องจดหมายที่ใช้การจัดส่งไดรฟ์คือ $2 USD ต่อข้อมูล 1 GB

For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).