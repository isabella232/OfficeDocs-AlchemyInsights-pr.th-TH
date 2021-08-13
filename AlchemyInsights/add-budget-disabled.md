---
title: เหตุใดปุ่มเพิ่มงบประมาณจึงถูกปิดใช้งาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954710"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>เหตุใดปุ่มเพิ่มงบประมาณจึงถูกปิดใช้งาน

เมื่อต้องการสร้างงบประมาณ คุณต้องมีหนึ่งในสิทธิ์ต่อไปนี้:

- กลุ่มการจัดการ การสมัครใช้งาน ขอบเขตกลุ่มทรัพยากร
- Cost Management Contributor
- เจ้าของ
- ผู้สนับสนุน
- เฉพาะลูกค้าระดับองค์กร: การลงทะเบียน แผนก ขอบเขตบัญชี
- ผู้ดูแลระบบการลงทะเบียน (ตั้งค่างบประมาณที่ ขอบเขตการลงทะเบียน)
- ผู้ดูแลระบบแผนก (ตั้งงบประมาณที่ขอบเขตแผนก)
- เจ้าของบัญชี (ตั้งค่างบประมาณที่ ขอบเขตบัญชี)
- ข้อตกลงของลูกค้าสมัยใหม่เท่านั้น: บัญชีการเรียกเก็บเงิน โปรไฟล์การเรียกเก็บเงิน ขอบเขตของส่วนใบแจ้งหนี้
- ผู้สร้างการสมัครใช้งาน Azure

**ฉันสร้างงบประมาณเมื่อค่าใช้จ่ายของฉันในเดือนปัจจุบันมีงบเกินงบแล้ว เหตุใดฉันจึงไม่ได้รับการแจ้งเตือน**  
ถ้าคุณเกินค่าเกณฑ์ต้นทุนที่ระบุแล้ว เมื่อคุณสร้างงบประมาณที่การแจ้งเตือนจะไม่เกิด เมื่อวงจรใหม่เริ่มต้น ถ้าคุณละเมิดค่าเกณฑ์ การแจ้งเตือนจะเริ่มต้น

**เมื่อใดที่ฉันควรได้รับการแจ้งเตือนหลังจากที่ฉันเกินค่าเกณฑ์การแจ้งเตือนงบประมาณที่กําหนดไว้ของฉัน**  
งบประมาณจะถูกประเมินทุกๆ 4 ชั่วโมง ซึ่งใช้เวลาอย่างน้อย 8 ชั่วโมงเพื่อให้ข้อมูลการใช้งานเข้าถึงระบบงบประมาณ เมื่อถึงเกณฑ์นี้ การแจ้งเตือนอาจใช้เวลานานถึง 12 ชั่วโมงเพื่อให้แจ้งเตือนหลังจากที่คุณเกินค่าเกณฑ์

**เหตุใดปุ่ม วันที่เริ่มต้น จึงถูกปิดใช้งานเมื่อฉันเลือกระยะเวลารีเซ็ตเดือนหรือเดือนการเรียกเก็บเงิน**  
งบประมาณจะสอดคล้องกับเดือนปฏิทินปัจจุบันหรือระยะเวลาการเรียกเก็บเงินปัจจุบัน (ในกรณีที่เลือก เดือนการเรียกเก็บเงิน) ดังนั้น เราจึงใส่ค่านี้ให้คุณล่วงหน้า

**เหตุใดฉันจึงไม่เห็นกราฟค่าใช้จ่ายของฉันในประสบการณ์การสร้างงบประมาณ**  
เราต้องการข้อมูลค่าใช้จ่ายอย่างน้อย 2 เดือนก่อนที่เราจะสามารถแสดงกราฟเพื่อช่วยคุณในการสร้างงบประมาณ

**เหตุใดฉันจึงไม่สามารถตั้งงบประมาณกับการสมัครใช้งานที่ฉันเพิ่งสร้าง**  
หลังจากการสร้างการสมัครใช้งาน ข้อมูลจะใช้เวลา 24-48 ชั่วโมงในการประมวลผลก่อนที่จะตั้งค่างบประมาณ

**แหล่งข้อมูล API งบประมาณ**

- [งบประมาณ API v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)ให้การดําเนินการเพื่อสร้างและอัปเดตงบประมาณ ด้วยการใช้ API งบประมาณ คุณสามารถตั้งค่าค่าเกณฑ์งบประมาณและกําหนดค่าการแจ้งเตือนหลายรายการให้แจ้งเตือนเมื่อคุณถึงเกณฑ์นั้น การแจ้งเตือนสามารถทริกเกอร์อีเมลหรือกลุ่มการปฏิบัติการของ Azure เพื่อใช้งานระบบอัตโนมัติ หมายเหตุ: การกรอง API นี้ไม่สอดคล้องกับการกรอง / มิติ API ของคิวรี
- [งบประมาณ API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): สร้างงบประมาณที่ความสามารถในการกรองค่าใช้จ่ายมากกว่า v1 การกรองจะจัดชิดสัญญาที่ใช้ใน API คิวรีและมิติของเรา นี่คืองบประมาณที่แนะนนะ API เพื่อใช้การเลื่อนไปข้างหน้า
- [ขนาด](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): ให้การดําเนินการเพื่อรับขนาดที่สนับสนุนการใช้งานของคุณภายใต้ขอบเขตที่หลากหลาย เมื่อใช้ API มิติ คุณสามารถเรียกใช้รายการของขนาดที่สามารถใช้เป็นข้อมูลป้อนเข้าในการสร้างคิวรีด้วย API คิวรี
- [คิว](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)รี : ให้การดําเนินการเพื่อรับข้อมูลค่าใช้จ่ายรวมและข้อมูลการใช้งานโดยยึดตามคิวรีที่คุณให้มา เมื่อใช้ API คิวรี คุณสามารถระบุการกรอง การเรียงล.ก. และการจัดกลุ่มตามขนาดที่พร้อมใช้งานทั้งหมดได้ (ซึ่งเข้าถึงได้จาก API มิติ)

**ต้นทุนที่พยากรณ์**

**เหตุใดฉันจึงไม่เห็นการคาดการณ์ค่าใช้จ่ายของฉันใน Cost Analysis**  
มีหลายสาเหตุที่การประมาณการคาดการณ์อาจหายไปให้คุณในการวิเคราะห์ต้นทุน บางส่วนมีดังต่อไปนี้:

1. ถ้าข้อมูลค่าใช้จ่ายของคุณเก่ากว่า 10 วัน แผนภูมิการพยากรณ์จะไม่โหลด ตัวแบบนี้ต้องการข้อมูลต้นทุนล่าสุดอย่างน้อย 10 วันเพื่อการฉายภาพที่ถูกต้อง
2. ถ้าคุณเลือกวันที่ประวัติศาสตร์ แผนภูมิการพยากรณ์จะไม่ปรากฏให้เห็น โปรดเลือกช่วงวันที่ที่มีวันที่ในอนาคตเพื่อให้แผนภูมิการพยากรณ์แสดงขึ้น
3. ถ้าบัญชีของคุณมีสกุลเงินหลายสกุลเงิน แผนภูมิการพยากรณ์จะเฉพาะต้นทุนโครงการของ 'ค่าใช้จ่ายทั้งหมดใน USD'

**เหตุใดการคาดการณ์จึงไม่เปลี่ยนแปลงเมื่อฉันเปลี่ยนแปลงทรัพยากรของฉัน**  
รูปแบบการพยากรณ์ต้องใช้เวลาสองสามวันเพื่อพิจารณาการเปลี่ยนแปลงในบัญชี และจะไม่คาดการณ์ในทันทีโดยยึดตามการเปลี่ยนแปลงในทรัพยากร  
หากต้องการเพิ่มหรือลดทรัพยากรในขั้นตอนที่มีขนาดใหญ่กว่า โมเดลจะใช้เวลาปรับกับการเปลี่ยนแปลงเหล่านี้นานกว่าเล็กน้อยเพื่อปรับค่า anomalies

**เหตุใดการคาดการณ์ของฉันจึงเพิ่มขึ้นหลังจากที่ฉันจองหรือซื้อ Marketplace**  
รูปแบบการพยากรณ์จะพิจารณา 'ค่าใช้จ่ายจริง' ของคุณ และไม่ใช่บัญชีการใช้งานและการซื้อแยกต่างหาก เมื่อซื้อแบบซื้อแล้วครั้งหนึ่ง โมเดลจะลดการประมาณค่าลงหลังจากผ่านไป 10 วันเพื่อนับค่าใช้จ่ายที่เพิ่มขึ้นทันที

**ฉันต้องการดูการคาดการณ์ของมิติเดียว (ตัวอย่างเช่น เมตร)**  
การคาดการณ์ในปัจจุบันสนับสนุนการประมาณค่าใช้จ่ายทั้งหมดไม่ใช่ที่วัดแต่ละเมตร ดังนั้น เมื่อ 'จัดกลุ่มตาม' มิติ การฉายภาพจะมีผลรวมของรายการทั้งหมดในมิติ

**เอกสารที่แนะนา**

- [Azure Cost Management คืออะไร](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [แนวทางปฏิบัติที่ดีที่สุดเกี่ยวกับ Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [วิเคราะห์ค่าใช้จ่ายและการใช้จ่ายของคุณ](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [สรวบและวิเคราะห์ต้นทุนด้วยการวิเคราะห์ต้นทุน](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: ราคา](https://azure.microsoft.com/services/cost-management/#pricing)
- [ตรวจสอบต้นทุนในการวิเคราะห์ต้นทุน](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [วิดีโอบทช่วยสอน: สร้างงบประมาณในพอร์ทัล Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [เบื้องต้นในการดูและการปรับแต่งงบประมาณ](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [สร้างและจัดการงบประมาณ](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [กําหนดค่าระบบอัตโนมัติด้วย Azure Action Groups และ API งบประมาณ](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [ใช้การแจ้งเตือนค่าใช้จ่ายเพื่อตรวจสอบการใช้งานและการใช้จ่าย](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [แนวทางปฏิบัติที่ดีที่สุดเกี่ยวกับการจัดการต้นทุน](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**วิดีโอบทช่วยสอน**

- [สร้างงบประมาณในพอร์ทัล Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [จัดการค่าใช้จ่ายด้วย API งบประมาณ และกลุ่มการปฏิบัติการ](https://go.microsoft.com/fwlink/?linkid=2147038)