---
title: ข้อผิดพลาดในการปิดการเชื่อมต่อSharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 0515ead28cdfdbdb9529c269b5170b294ab2b120
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543056"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="06c15-102">ข้อผิดพลาด "การเชื่อมต่อที่ขีดเส้นใต้ถูกปิด" SharePoint</span><span class="sxs-lookup"><span data-stu-id="06c15-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="06c15-103">ถ้าคุณได้รับข้อผิดพลาด "การเชื่อมต่อที่ขีดเส้นใต้ถูกปิด" SharePointอาจเกี่ยวข้องกับการเลิกใช้ TLS 1.0/1.1</span><span class="sxs-lookup"><span data-stu-id="06c15-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="06c15-104">ดูข้อมูลเพิ่มเติมที่บทความเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="06c15-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="06c15-105">การเตรียม 1.2 TLS ในOffice 365 Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="06c15-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="06c15-106">ข้อผิดพลาดการรับรองความถูกต้องจะเกิดขึ้นถ้าไคลเอ็นต์ไม่มีการสนับสนุน TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="06c15-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="06c15-107">อัปเดตเพื่อเปิดใช้งาน TLS 1.1 และ TLS 1.2 เป็นโพรโทคอลที่ปลอดภัยเริ่มต้นใน WinHTTP Windows</span><span class="sxs-lookup"><span data-stu-id="06c15-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="06c15-108">ถ้าผู้ใช้อยู่ในWindows 7 ตรวจสอบให้แน่ใจว่า พวกเขาตรวจสอบชุดการเข้ารหัส[TLS Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)</span><span class="sxs-lookup"><span data-stu-id="06c15-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>