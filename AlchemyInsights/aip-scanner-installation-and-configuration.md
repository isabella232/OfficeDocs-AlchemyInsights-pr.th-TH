---
title: 'เครื่องสแกนเนอร์ AIP: การติดตั้งและการกําหนดค่า'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358568"
---
# <a name="aip-scanner-installation-and-configuration"></a>เครื่องสแกนเนอร์ AIP: การติดตั้งและการกําหนดค่า

**ในการติดตั้งเครื่องสแกน AIP ให้ทําตามคําแนะนําที่แนะนํา**:

1. ถ้าคุณกําลังปรับรุ่น และไม่ทําการติดตั้งใหม่ทั้งหมด โปรดตรวจสอบให้แน่ใจว่าคุณได้ปฏิบัติตามคําแนะนําสําหรับ[การปรับรุ่นสแกนเนอร์การป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)และสําหรับไคลเอนต์การติดฉลากแบบรวม[upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. ตรวจสอบว่าคุณปฏิบัติตาม[ข้อกําหนดของไฟร์วอลล์และการตั้งค่าโครงสร้างพื้นฐานเครือข่าย](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)ทั้งหมด
3. ตรวจสอบว่านโยบายของคุณ[ถูกตั้งค่า](https://docs.microsoft.com/azure/information-protection/configure-policy)เป็นป้ายกํากับอัตโนมัติหรือมีป้ายกํากับเริ่มต้นในนโยบาย
4. ตรวจสอบให้แน่ใจว่า มีการกําหนดค่าชนิดแฟ้มที่เกี่ยวข้องสําหรับป้ายชื่อ/การป้องกันตามที่อธิบายไว้ใน[ชนิดแฟ้มได้รับการสนับสนุน โดยไคลเอ็นต์การป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) นอกจากนี้ ถ้าคุณต้องการเปลี่ยนลักษณะการทํางานเริ่มต้น ให้ทําตามคําแนะนําเหล่านี้:[การเปลี่ยนระดับการป้องกันเริ่มต้นของแฟ้ม](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. ตรวจสอบว่า บัญชีผู้ใช้ที่กําหนดค่าให้เรียกใช้บริการสแกนเนอร์มีสิทธิ์ในการเข้าถึงที่เก็บที่กําหนดค่าไว้ทั้งหมด
6. หากคุณยังพบปัญหาโปรดส่งออกบันทึกของสแกนเนอร์และเพิ่มไปยังตั๋วสนับสนุนของคุณ

**ส่งออกแฟ้มบันทึกของสแกนเนอร์การป้องกันข้อมูล Azure**

1. นําทางไปยัง %localappdata%\Microsoft\MSIP ภายใต้บริบทของผู้ใช้ที่เรียกใช้บริการสแกนเนอร์
2. ซิปเนื้อหาทั้งหมดภายใต้โฟลเดอร์ MSIP
3. บันทึกบันทึกไปยังตําแหน่งที่คุณเลือกและแนบกับคําขอบริการของคุณ
4. คุณยังสามารถใช้[การส่งออก AIPLogs - onbehalf ของ](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**สําหรับข้อมูลเพิ่มเติม โปรดดูที่**:
- [การปรับใช้สแกนเนอร์การป้องกันข้อมูล Azure โดยอัตโนมัติจัดประเภท และป้องกันแฟ้ม](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [ระบุและใช้พารามิเตอร์โทเค็นสําหรับชุด AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [เรียกใช้รอบการค้นพบและดูรายงานสําหรับสแกนเนอร์](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [ตรวจทานเอกสารประกอบการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ข้อกําหนดสําหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูลของ Azure](https://www.microsoft.com/download/details.aspx?id=53018)
