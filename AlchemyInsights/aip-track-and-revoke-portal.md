---
title: 'AIP: ติดตามและยกเลิกพอร์ทัล'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002281"
- "5519"
ms.openlocfilehash: 32cd346c9af145f733b0a62746a0ee1b632fa5ab
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358520"
---
# <a name="aip-track-and-revoke-portal"></a><span data-ttu-id="19398-102">AIP: ติดตามและยกเลิกพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="19398-102">AIP: Track and revoke portal</span></span>

<span data-ttu-id="19398-103">ใช้**ไซต์การติดตามเอกสาร**ในพอร์ทัล Azure เพื่อติดตาม และยกเลิกเอกสารเมื่อใช้การป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="19398-103">Use the **document tracking site** in the Azure Portal to track and revoke documents when using Azure Information Protection.</span></span> <span data-ttu-id="19398-104">แอปพลิเคชัน Office (Word, Excel และ PowerPoint) และ File Explorer ยังสามารถใช้เพื่อติดตามและยกเลิกเอกสารได้</span><span class="sxs-lookup"><span data-stu-id="19398-104">The Office applications (Word, Excel and PowerPoint) and File Explorer can also be used to track and revoke documents.</span></span>

1. <span data-ttu-id="19398-105">ในไซต์การติดตามเอกสาร ให้คลิก**เพิกถอนการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="19398-105">In the document tracking site, click **Revoke access**.</span></span> <span data-ttu-id="19398-106">การเพิกถอนเอกสารจะลบการเข้าถึงจากผู้ใช้ที่ได้รับอนุญาต เอกสารจะไม่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="19398-106">Revoking a document removes access from authorized users; the document is not deleted.</span></span>
2. <span data-ttu-id="19398-107">ในโปรแกรมประยุกต์ Office:</span><span class="sxs-lookup"><span data-stu-id="19398-107">In the Office application:</span></span>
    - <span data-ttu-id="19398-108">เปิดเอกสารที่มีการป้องกันที่คุณต้องการติดตามหรือยกเลิก</span><span class="sxs-lookup"><span data-stu-id="19398-108">Open the protected document that you want to track or revoke.</span></span>
    - <span data-ttu-id="19398-109">บนแท็บ**หน้าแรก**ในกลุ่ม**การป้องกัน**ให้คลิก**ป้องกันแทร็ก>และเพิกถอน**</span><span class="sxs-lookup"><span data-stu-id="19398-109">On the **Home** tab, in the **Protection** group, click **Protect > Track and Revoke**.</span></span>

- <span data-ttu-id="19398-110">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการติดตามและเพิกถอนเอกสาร ให้ดูที่[การติดตามและเพิกถอน](https://docs.microsoft.com/azure/information-protection/rms-client/client-track-revoke)</span><span class="sxs-lookup"><span data-stu-id="19398-110">For additional information on tracking and revoking a document, see [Track and Revoke](https://docs.microsoft.com/azure/information-protection/rms-client/client-track-revoke).</span></span>

<span data-ttu-id="19398-111">สําหรับข้อมูลเกี่ยวกับการใช้ PowerShell เพื่อจัดการไซต์การติดตามเอกสาร</span><span class="sxs-lookup"><span data-stu-id="19398-111">For information on using PowerShell to manage the document tracking site, logging information, see the following:</span></span>
- [<span data-ttu-id="19398-112">คู่มือผู้ใช้: ติดตาม และยกเลิกเอกสารของคุณเมื่อคุณใช้การป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="19398-112">User Guide: Track and revoke your documents when you use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-track-revoke)
- [<span data-ttu-id="19398-113">คู่มือผู้ดูแลระบบ: การกําหนดค่าและการใช้การติดตามเอกสารสําหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="19398-113">Admin Guide: Configuring and using document tracking for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-document-tracking)
- [<span data-ttu-id="19398-114">ใบอนุญาตการใช้สิทธิ์การจัดการสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="19398-114">Rights Management use license</span></span>](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#rights-management-use-license)
- [<span data-ttu-id="19398-115">ตรวจทานการสมัครใช้งานและคุณลักษณะการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="19398-115">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- [<span data-ttu-id="19398-116">ข้อกําหนดสําหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="19398-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="19398-117">บทแนะนําการเริ่มต้นอย่างรวดเร็วสําหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="19398-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
