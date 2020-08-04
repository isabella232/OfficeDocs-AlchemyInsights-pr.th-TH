---
title: ใช้การบันทึกการใช้งานสําหรับการจัดการสิทธิ์ Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556024"
---
# <a name="use-usage-logging-for-azure-rights-management"></a>ใช้การบันทึกการใช้งานสําหรับการจัดการสิทธิ์ Azure

โดยค่าเริ่มต้น การบันทึกการใช้งานการป้องกันถูกเปิดใช้งานสําหรับลูกค้าทั้งหมด บันทึกถูกเขียนเป็นชุดของ blobs ในที่เก็บข้อมูล Azure สําหรับผู้เช่าของคุณ หลังจากการดําเนินการป้องกันอาจใช้เวลาถึง 15 นาทีเพื่อให้บันทึกส่วนใหญ่ปรากฏขึ้น

คุณสามารถใช้บันทึกการใช้งานการป้องกันเพื่อ:

- วิเคราะห์ข้อมูลเชิงลึกทางธุรกิจ

- ตรวจสอบการละเมิด

- ดําเนินการวิเคราะห์ทางนิติเวช

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การบันทึกและการวิเคราะห์การใช้งานการป้องกันจากการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/log-analyze-usage)

สําหรับข้อมูลเกี่ยวกับการบันทึกการใช้งานไคลเอ็นต์ ให้ดูที่[คู่มือผู้ดูแลระบบ: แฟ้มไคลเอ็นต์การป้องกันข้อมูล Azure และการบันทึกการใช้งานไคลเอ็นต์](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging)

สําหรับข้อมูลเพิ่มเติม โปรดดู:

- [ข้อกําหนดในการปกป้องข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
    
- [บทช่วยสอน: กําหนดค่าการตั้งค่านโยบายการป้องกันข้อมูล Azure และสร้างป้ายชื่อใหม่](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)