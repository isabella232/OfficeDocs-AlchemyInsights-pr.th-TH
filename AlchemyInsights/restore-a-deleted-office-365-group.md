---
title: คืนค่ากลุ่มMicrosoft 365ที่ถูกลบ
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959045"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>คืนค่ากลุ่มMicrosoft 365ที่ถูกลบ

คุณสามารถคืนค่ากลุ่มที่ถูกลบMicrosoft 365หรือMicrosoft Teamsภายใน 30 วันจากการลบ

1. ไปที่[ศูนย์การจัดการ Microsoft 365](https://aka.ms/RestoreDeletedGroup)เพื่อเข้าสู่ระบบรายการของคุณคือกลุ่มและทีมที่ถูกลบ

    **หมายเหตุ:** เข้าสู่ระบบโดยใช้บัญชีที่มอบหมายให้ผู้ดูแลผู้เช่าหรือบทบาทผู้ดูแลกลุ่ม

1. เลือกกลุ่มMicrosoft 365/Teamsที่ถูกลบแล้วคลิก **คืนค่า** กลุ่ม

    ถ้ากลุ่มไม่สามารถคืนค่าได้เนื่องจากที่อยู่ SMTP ที่ขัดแย้งกัน ให้ใช้สั่งต่อไปนี้เพื่อค้นหาวัตถุที่ทําให้เกิดข้อขัดแย้งและเอาที่อยู่ SMTP ออก:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **หมายเหตุ:** ในบางกรณี อาจใช้เวลาถึง 24 ชั่วโมงในการคืนค่ากลุ่มและข้อมูลทั้งหมด

    For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).