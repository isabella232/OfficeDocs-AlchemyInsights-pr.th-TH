---
title: 'การสแกน AIP: การติดตั้งและการกำหนดค่า'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686661"
---
# <a name="aip-scanner-installation-and-configuration"></a>การสแกน AIP: การติดตั้งและการกำหนดค่า

**เมื่อต้องการติดตั้งสแกนเนอร์ AIP ให้ทำตามแนวทางที่แนะนำ**:

1. ถ้าคุณกำลังอัปเกรดและไม่ได้ทำการติดตั้งใหม่ทั้งหมดโปรดตรวจสอบให้แน่ใจว่าคุณได้ทำตามแนวทางสำหรับการ[อัปเกรดสแกนเนอร์การป้องกันข้อมูลของ azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)และสำหรับไคลเอ็นต์การติดฉลากแบบรวมให้ดู[ที่การอัปเกรดสแกนเนอร์การป้องกันข้อมูลของ azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. ตรวจสอบว่าคุณสอดคล้องกับ [ไฟร์วอลล์และความต้องการตั้งค่าโครงสร้างพื้นฐานของเครือข่าย](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)ทั้งหมด
3. ตรวจสอบให้แน่ใจว่านโยบายของคุณ [ถูกตั้งค่า](https://docs.microsoft.com/azure/information-protection/configure-policy) เป็นการติดฉลากอัตโนมัติหรือมีป้ายชื่อเริ่มต้นในนโยบาย
4. ตรวจสอบให้แน่ใจว่าชนิดไฟล์ที่เกี่ยวข้องถูกกำหนดค่าสำหรับป้ายชื่อ/การป้องกันตามที่อธิบายไว้ใน[ชนิดไฟล์ที่ได้รับการสนับสนุนโดยไคลเอ็นต์การป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) นอกจากนี้ถ้าคุณต้องการเปลี่ยนลักษณะการทำงานเริ่มต้นให้ทำตามแนวทางเหล่านี้:[การเปลี่ยนระดับการป้องกันเริ่มต้นของไฟล์](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. ตรวจสอบว่าบัญชีผู้ใช้ที่ได้รับการกำหนดค่าให้เรียกใช้บริการสแกนเนอร์มีสิทธิ์ในการเข้าถึงที่เก็บที่กำหนดค่าไว้ทั้งหมด
6. ถ้าคุณยังคงประสบปัญหาโปรดส่งออกบันทึกของสแกนเนอร์และเพิ่มไฟล์เหล่านั้นลงในตั๋วสนับสนุนของคุณ

**ส่งออกบันทึกสแกนเนอร์การป้องกันข้อมูล Azure**

1. นำทางไปยัง%localappdata%\Microsoft\MSIP ภายใต้บริบทของผู้ใช้ที่กำลังเรียกใช้บริการสแกนเนอร์
2. Zip เนื้อหาทั้งหมดภายใต้โฟลเดอร์ MSIP
3. บันทึกไฟล์บันทึกไปยังตำแหน่งที่ตั้งของคุณและแนบเข้ากับคำขอบริการของคุณ
4. นอกจากนี้คุณยังสามารถใช้การ[ส่งออก-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**สำหรับข้อมูลเพิ่มเติมให้ดู**ที่:
- [การปรับใช้สแกนเนอร์การป้องกันข้อมูลของ Azure เพื่อจัดประเภทและป้องกันไฟล์โดยอัตโนมัติ](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [ระบุและใช้พารามิเตอร์โทเค็นสำหรับการตั้งค่า-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [การเรียกใช้วงจรการค้นหาและดูรายงานสำหรับสแกนเนอร์](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [ตรวจทานเอกสารประกอบการป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [ข้อกำหนดสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure](https://www.microsoft.com/download/details.aspx?id=53018)
