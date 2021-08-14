---
title: พอร์ตส่วนขยาย Google Chrome Microsoft Edge (Chromium)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
- "8297"
- "9004617"
ms.openlocfilehash: 34ec7e71a2f27eb5b46395876a4d1c903189be1050e523796c9f2a817c20aaa0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973716"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>พอร์ตส่วนขยาย Google Chrome Microsoft Edge (Chromium)

เป็นเรื่องง่ายที่จะพอร์ตส่วนขยาย[Google Chrome เพื่อMicrosoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension) ในกรณีส่วนใหญ่ คุณเพียงต้องเปลี่ยนแปลงน้อยที่สุดเพื่อเรียกใช้ส่วนขยายเหล่านี้Microsoft Edge

API ส่วนขยายและคีย์รายการที่ได้รับการสนับสนุนโดย Google Chrome เข้ากันได้กับMicrosoft Edge อย่างไรก็ตาม Microsoft Edge API ส่วนขยาย chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken และ chrome.instanceID