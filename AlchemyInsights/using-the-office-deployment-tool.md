---
title: ใช้เครื่องมือการปรับใช้ Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493271"
---
# <a name="using-the-office-deployment-tool-odt"></a>ใช้เครื่องมือการปรับใช้ Office (ODT)

คุณสามารถใช้เครื่องมือการปรับใช้ Office (ODT) เพื่อปรับใช้ Office รุ่น Office 365 เครื่องมือการปรับใช้ Office (setup.exe) ถูกเรียกใช้จากบรรทัดคำสั่ง และใช้แฟ้ม XML การกำหนดค่าการตั้งค่าใดที่จะนำไปใช้เมื่อปรับใช้ Office
  
1. ดาวน์โหลดเครื่องมือการปรับใช้ Office รุ่นล่าสุดจาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](http://go.microsoft.com/fwlink/p/?LinkID=626065)
    
2. ใช้เครื่อง[มือกำหนดเอง Office (OCT)](https://config.office.com)เพื่อเลือกการกำหนดลักษณะของคุณปรับใช้ และสร้างแฟ้ม XML การกำหนดค่า แฟ้มการกำหนดค่าการส่งออก และวางไว้ในโฟลเดอร์เดียวกับที่ setup.exe ที่ตั้งอยู่ภายในเครื่อง 
    
    **หมายเหตุ:** การติดตั้ง office ออกใช้โดยทั่วไปเกิดขึ้นครบกำหนดเพื่อ misconfigured หรือ malformatted แฟ้มการตั้งค่าคอนฟิก เมื่อต้องการหลีกเลี่ยงปัญหาดังกล่าว เราขอแนะนำให้ คุณใช้เครื่องมือกำหนดเองของ Office เมื่อต้องการสร้างแฟ้มการกำหนดค่า คุณยังสามารถนำเข้าแฟ้มการกำหนดค่าที่มีอยู่ลงในเครื่องมือกำหนดเองของ Office 
    
3. จากพร้อมท์คำสั่ง สลับไปยังตำแหน่งที่ตั้งที่ setup.exe และเรียกใช้เครื่องมือการปรับใช้ Office ในโหมดดาวน์โหลด และระบุแฟ้มการกำหนดค่าที่คุณเพิ่งบันทึก ในตัวอย่างนี้ แฟ้มการกำหนดค่าถูกตั้งชื่อว่า Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. เรียกใช้เครื่องมือการปรับใช้ Office ในโหมดที่ตั้งค่าคอนฟิก และระบุแฟ้มการกำหนดค่า
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **หมายเหตุ:** คุณต้องเรียกใช้ขั้นตอนนี้จากคอมพิวเตอร์ไคลเอนต์ที่คุณต้องการติดตั้ง Office และคุณต้องมีสิทธิ์เป็นผู้ดูแลท้องถิ่นบนคอมพิวเตอร์เครื่องนั้น 
    
เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการใช้เครื่องมือการปรับใช้ Office สำหรับสถานการณ์การปรับใช้ Office 365 ProPlus ของคุณ ดู[ภาพรวมของเครื่องมือการปรับใช้ Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool) สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการใช้เครื่องมือกำหนดเอง Office ดู[ภาพรวมของเครื่องมือการกำหนดเองของ Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
  

