---
title: แก้ไขปัญหารหัสข้อผิดพลาด AADSTS650056
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9803"
- "9005744"
ms.openlocfilehash: 945be2b496b98937bfae6d1f573162d1f2ebb4b6
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038039"
---
# <a name="troubleshoot-error-code-aadsts650056"></a><span data-ttu-id="f52e6-102">แก้ไขปัญหารหัสข้อผิดพลาด AADSTS650056</span><span class="sxs-lookup"><span data-stu-id="f52e6-102">Troubleshoot error code AADSTS650056</span></span>

<span data-ttu-id="f52e6-103">เมื่อต้องการแก้ไขข้อผิดพลาด AADSTS650056 ให้ปฏิบัติตามขั้นตอนที่แนะนาด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="f52e6-103">To resolve AADSTS650056 error, perform the below recommended step.</span></span>

<span data-ttu-id="f52e6-104">**AADSTS65005**: MisconfiguredApplication - รายการการเข้าถึงทรัพยากรที่แอปต้องมีไม่มีแอปที่ทรัพยากรหรือแอปไคลเอ็นต์ร้องขอการเข้าถึงทรัพยากร ซึ่งไม่ได้ระบุไว้ในรายการการเข้าถึงทรัพยากรหรือบริการ Graph ที่ส่งกลับการร้องขอที่ไม่ดีหรือแหล่งข้อมูลที่ไม่พบ</span><span class="sxs-lookup"><span data-stu-id="f52e6-104">**AADSTS65005**: MisconfiguredApplication - The app required resource access list does not contain apps discoverable by the resource or The client app has requested access to resource, which was not specified in its required resource access list or Graph service returned bad request or resource not found.</span></span> <span data-ttu-id="f52e6-105">ถ้าแอปสนับสนุน SAML คุณอาจกําหนดค่าแอปด้วยตัวระบุ (เอนทิตี) ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="f52e6-105">If the app supports SAML, you may have configured the app with the wrong Identifier (Entity).</span></span>

<span data-ttu-id="f52e6-106">For more information, see the troubleshooting article for error [AADSTS650056](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts650056-misconfigured-app).</span><span class="sxs-lookup"><span data-stu-id="f52e6-106">For more information, see the troubleshooting article for error [AADSTS650056](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts650056-misconfigured-app).</span></span>
