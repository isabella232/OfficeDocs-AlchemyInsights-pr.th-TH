---
title: Active Directory ไม่ซิงค์
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937120"
---
# <a name="active-directory-not-syncing"></a>Active Directory ไม่ซิงค์

ถ้าคุณได้รับข้อผิดพลาดการซิงโครไนซ์ เช่น "ไม่มีการซิงโครไนซ์ล่าสุด" หรือสังเกตสถานะการซิงโครไนซ์ไดเรกทอรีในพอร์ทัลผู้ดูแลระบบของ Office ระบุว่า "ซิงค์ครั้งล่าสุดนานกว่า 3 วันที่ผ่านมา" อาจเป็นเพราะ AADConnect มีการตั้งค่าที่ไม่ถูกต้องหรือมีสิทธิ์ที่ไม่เพียงพอที่จะซิงโครไนซ์ได้  

การติดตั้ง AADConnect อีกครั้งโดยใช้การตั้งค่าแบบด่วนอาจช่วยแก้ไขปัญหาได้อย่างรวดเร็ว ดังนี้

1. [ดาวน์โหลด AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)เวอร์ชันล่าสุด

2. [ให้ปฏิบัติตามคําแนะนําในการติดตั้ง](/azure/active-directory/hybrid/how-to-connect-install-express)แบบด่วน

ต้องเชื่อมต่อ Azure AD Windows Server 2012 หรือใหม่กว่า เซิร์ฟเวอร์นี้ต้องถูกรวมโดเมนและอาจเป็นตัวควบคุมโดเมนหรือเซิร์ฟเวอร์สมาชิก For a full list of Azure AD เชื่อมต่อ requirements and pre-requisites, review [Prerequisites for Azure AD เชื่อมต่อ](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

For more information about AADConnect service accounts, see [Azure AD เชื่อมต่อ: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
