---
title: Device Writeback
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
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256971"
---
# <a name="device-writeback"></a>Device Writeback

ใช้ Device Writeback ในสถานการณ์ต่อไปนี้:

- เปิดใช้งาน [Windows Hello for Business โดยใช้การปรับใช้ใบรับรองความเชื่อถือแบบไฮบริด](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- เปิดใช้งานการเข้าถึงตามเงื่อนไขโดยยึดตามอุปกรณ์ไปยังแอปพลิเคชันที่ได้รับการป้องกัน ADFS (2012 R2 หรือสูงกว่า) (ใช้ความน่าเชื่อถือของบริษัท)

    > [!NOTE]
    > การสมัครใช้งาน Azure AD Premium จะต้องใช้ในการเขียนข้อมูลอุปกรณ์

This provides additional security and assurance that access to applications is granted only to trusted devices. For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and Setting up [On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).

For more information on Enableing Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
