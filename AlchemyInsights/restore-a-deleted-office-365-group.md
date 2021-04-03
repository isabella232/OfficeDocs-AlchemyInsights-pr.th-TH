---
title: คืนค่ากลุ่ม Microsoft 365 ที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505729"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>คืนค่ากลุ่ม Microsoft 365 ที่ถูกลบ

คุณสามารถคืนค่ากลุ่ม Microsoft 365 หรือ Microsoft Teams ที่ถูกลบภายใน 30 วันจากการลบ

1. เมื่อต้องการเข้าสู่ระบบศูนย์การจัดการ Microsoft 365 และแสดงรายการกลุ่มและทีมที่ถูกลบ ให้ไปที่ศูนย์การจัดการ[Microsoft 365](https://aka.ms/RestoreDeletedGroup)

    **หมายเหตุ:** เข้าสู่ระบบโดยใช้บัญชีที่มอบหมายให้ผู้ดูแลระบบผู้เช่าหรือบทบาทผู้ดูแลกลุ่ม

1. เลือกกลุ่ม Microsoft 365/Teams ที่ถูกลบเพื่อคืนค่าและคลิก **กลุ่ม** คืนค่า

    ถ้ากลุ่มไม่สามารถคืนค่าได้เนื่องจากที่อยู่ SMTP ที่ขัดแย้งกัน ให้ใช้สั่งต่อไปนี้เพื่อค้นหาวัตถุที่ทําให้เกิดข้อขัดแย้งและเอาที่อยู่ SMTP ออก

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **หมายเหตุ:** ในบางกรณี อาจใช้เวลาถึง 24 ชั่วโมงในการคืนค่ากลุ่มและข้อมูลทั้งหมด

    For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).