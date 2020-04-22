---
title: ป้ายแสดงความละเอียดอ่อนไม่ปรากฏ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 72dc88a55b55954f34c95fa5b5038f472261c5bb
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758535"
---
# <a name="sensitivity-labels-not-appearing"></a>ป้ายแสดงความละเอียดอ่อนไม่ปรากฏ

ป้ายแสดงความไวช่วยให้คุณสามารถจําแนกและช่วยปกป้องเนื้อหาที่ละเอียดอ่อนของคุณ พวกเขาสามารถสร้างขึ้นในศูนย์การปฏิบัติตามกฎระเบียบของ Microsoft 365 ศูนย์รักษาความปลอดภัย Microsoft 365 หรือความปลอดภัยของ Microsoft 365 &ศูนย์การปฏิบัติตามกฎระเบียบภายใต้การจําแนก>ป้ายความไว เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับคุณลักษณะนี้ ให้ดูที่[ภาพรวมของป้ายชื่อระดับความลับ](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)

ถ้าคุณกําหนดค่าป้ายความละเอียดอ่อนของคุณ แต่จะไม่ปรากฏในแอป Office ให้ตรวจสอบดังต่อไปนี้

- ยืนยันว่าได้[เผยแพร่](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do)ป้ายชื่อระดับความลับไปยังผู้ใช้และกลุ่มที่คุณต้องการแล้ว

- ยืนยันว่าผู้ใช้กําลังใช้แอปที่สนับสนุนป้ายความละเอียดอ่อน[sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- ถ้าคุณกําลัง[โยกย้ายป้ายชื่อการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)ให้ระวังข้อควรพิจารณาที่แสดง[ไว้ที่นี่](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- การสนับสนุนการป้องกันข้อมูลสูญหาย (DLP): ปัจจุบัน เฉพาะป้ายผนึกที่เก็บข้อมูลเท่านั้นที่สามารถใช้เป็นเงื่อนไขในนโยบาย DLP ได้  การสนับสนุนสําหรับป้ายกํากับความไวในนโยบาย DLP ยังไม่พร้อมใช้งาน แต่เรากําลังทํางานกับมัน

- เมื่อเปิดใช้งานการเข้ารหัสลับบนป้ายชื่อระดับความลับ
    - กําหนดสิทธิ์เดี๋ยวนี้
    - อนุญาตให้ผู้ใช้กําหนดสิทธิ์


สําหรับข้อมูลเพิ่มเติมเกี่ยวกับปัญหาที่เป็นไปได้ ให้ดูที่[ปัญหาที่ทราบเกี่ยวกับป้ายชื่อระดับความลับ](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)