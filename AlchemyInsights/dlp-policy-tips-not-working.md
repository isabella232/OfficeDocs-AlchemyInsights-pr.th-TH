---
title: เคล็ดลับนโยบาย DLP ไม่ใช้งาน
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958721"
---
# <a name="dlp-policy-tip-issues"></a>ปัญหาเคล็ดลับนโยบาย DLP

**สิ่ง** สําคัญ: ระหว่างช่วงเวลาที่ไม่มีประวัติใช้งานเหล่านี้ เราปฏิบัติตามขั้นตอนเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่ โปรดเยี่ยมชม การปรับฟีเจอร์ชั่วคราวของ [SharePoint Online](https://aka.ms/ODSPAdjustments) เพื่อดูข้อมูลเพิ่มเติม

เมื่อต้องการกําหนดค่าเคล็ดลับนโยบายเกี่ยวกับนโยบาย DLP ของคุณ&ศูนย์การปฏิบัติตามข้อบังคับในโหมดการบังคับใช้ทั้งหมด ให้ปฏิบัติดังนี้

- ตรวจสอบให้แน่ใจว่ามีการเปิดใช้งาน **เคล็ดลับ** นโยบายในกฎ DLP แล้ว For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).

- ตรวจสอบให้แน่ใจว่าเนื้อหาของคุณตรงกับสิ่งที่ต้องระบุเพื่อทริกเกอร์กฎที่ระบุไว้ในข้อนิยาม[เอนทิตีของชนิดข้อมูลที่เป็นความลับ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- เคล็ดลับนโยบายจะแสดงทั้งใน OWA และ Outlook อย่างไรก็ตาม เมื่อใช้ Outlook 2013 หรือใหม่กว่า เคล็ดลับนโยบายจะแสดงภายใต้เงื่อนไขบางอย่างเท่านั้น For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).

For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).