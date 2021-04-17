---
title: 'ตัวสแกน AIP: การติดตั้งและการกําหนดค่า'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821682"
---
# <a name="aip-scanner-installation-and-configuration"></a>ตัวสแกน AIP: การติดตั้งและการกําหนดค่า

**เมื่อต้องการติดตั้งสแกนเนอร์ AIP ให้ปฏิบัติตามแนวทางที่แนะนํา**:

1. ถ้าคุณอัปเกรดและไม่ได้ติดตั้งใหม่ทั้งหมด โปรดตรวจสอบให้แน่ใจว่าคุณได้ปฏิบัติตามแนวทางการอัปเกรดตัวสแกน Azure Information [Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)และไคลเอ็นต์การลงป้ายแบบรวมศูนย์ ให้ดู การอัปเกรดตัวสแกน[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. ตรวจสอบว่าคุณปฏิบัติตามข้อกฎหมาย [การตั้งค่าไฟร์วอลล์และโครงสร้างพื้นฐานของเครือข่าย](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)ทั้งหมด
3. ตรวจสอบให้แน่ใจว่า [นโยบายของคุณถูกตั้งค่า](https://docs.microsoft.com/azure/information-protection/configure-policy) ให้ติดป้ายผนึกอัตโนมัติหรือมีป้ายชื่อเริ่มต้นในนโยบาย
4. ตรวจสอบให้แน่ใจว่าชนิดไฟล์ที่เกี่ยวข้องได้รับการกําหนดค่าไว้ป้ายชื่อ/การป้องกันตามที่อธิบายไว้[ใน ชนิดไฟล์ ที่สนับสนุนโดยไคลเอ็นต์ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) นอกจากนี้ ถ้าคุณต้องการเปลี่ยนลักษณะการรักษาความปลอดภัยเริ่มต้น ให้ปฏิบัติตามแนวทาง [เหล่านี้: การเปลี่ยนระดับการป้องกันเริ่มต้นของ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)ไฟล์
5. ตรวจสอบว่าบัญชีผู้ใช้ที่กําหนดค่าให้เรียกใช้บริการสแกนเนอร์มีสิทธิ์ในการเข้าถึงที่เก็บที่กําหนดค่าไว้ทั้งหมด
6. ถ้าคุณยังคงพบปัญหา โปรดส่งออกบันทึกสแกนเนอร์และเพิ่มบันทึกลงในตั๋วการสนับสนุนของคุณ

**ส่งออกบันทึก Azure Information Protection Scanner**

1. นําทางไปยัง %localappdata%\Microsoft\MSIP ภายใต้บริบทของผู้ใช้ที่เรียกใช้บริการสแกนเนอร์
2. Zip เนื้อหาทั้งหมดภายใต้โฟลเดอร์ MSIP
3. บันทึกแฟ้มบันทึกไปยังตัวเลือกของสถานที่และแนบไฟล์กับการร้องขอบริการของคุณ
4. คุณยังสามารถใช้[Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**หากต้องการข้อมูลเพิ่มเติม โปรดดู**:
- [การปรับใช้ตัวสแกน Azure Information Protection เพื่อจัดประเภทและปกป้องไฟล์โดยอัตโนมัติ](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [ระบุและใช้พารามิเตอร์โทเค็นใน Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [เรียกใช้รอบการค้นพบและดูรายงานของสแกนเนอร์](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [ตรวจทานเอกสาร Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ความต้องการของ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [ดาวน์โหลดไคลเอ็นต์ Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
