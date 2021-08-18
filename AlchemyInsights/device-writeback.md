---
title: Writeback ของอุปกรณ์
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320105"
---
# <a name="device-writeback"></a>Writeback ของอุปกรณ์

ใช้ Device Writeback ในสถานการณ์ต่อไปนี้:

- เปิดใช้งาน[Windows Hello for Business โดยใช้การปรับใช้ใบรับรองความเชื่อถือแบบไฮบริด](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- เปิดใช้งานการเข้าถึงตามเงื่อนไขตามอุปกรณ์ไปยังแอปพลิเคชันที่ได้รับการป้องกัน ADFS (2012 R2 หรือสูงกว่า) (ขึ้นอยู่กับความเชื่อถือของบริษัท)

    **หมายเหตุ**: ต้องมีการสมัครใช้งาน Azure AD Premiumการเขียนกลับของอุปกรณ์

This provides additional security and assurance that access to applications is granted only to trusted devices. For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and Setting up [On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).

For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
