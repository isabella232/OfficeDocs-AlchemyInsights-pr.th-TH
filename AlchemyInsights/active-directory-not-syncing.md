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
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314223"
---
# <a name="active-directory-not-syncing"></a>Active Directory ไม่ซิงค์

ถ้าคุณได้รับข้อผิดพลาดการซิงโครไนซ์ เช่น "ไม่มีการซิงโครไนซ์ล่าสุด" หรือสังเกตสถานะการซิงโครไนซ์ไดเรกทอรีในพอร์ทัลผู้ดูแลระบบของ Office ระบุว่า "ซิงค์ครั้งล่าสุดนานกว่า 3 วันที่ผ่านมา" อาจเป็นเพราะ AADConnect มีการตั้งค่าที่ไม่ถูกต้องหรือมีสิทธิ์ไม่เพียงพอที่จะซิงค์ได้  

การติดตั้ง AADConnect อีกครั้งโดยใช้การตั้งค่าแบบด่วนอาจช่วยแก้ไขปัญหาได้อย่างรวดเร็ว ดังนี้

1. [ดาวน์โหลด AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)เวอร์ชันล่าสุด

2. [ให้ปฏิบัติตามคําแนะนําในการติดตั้ง](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)แบบด่วน

ต้องเชื่อมต่อ Azure AD Windows Server 2012 หรือใหม่กว่า เซิร์ฟเวอร์นี้ต้องถูกรวมโดเมนและอาจเป็นตัวควบคุมโดเมนหรือเซิร์ฟเวอร์สมาชิก For a full list of Azure AD เชื่อมต่อ requirements and pre-requisites, review [Prerequisites for Azure AD เชื่อมต่อ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

For more information about AADConnect service accounts, see [Azure AD เชื่อมต่อ: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
