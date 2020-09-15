---
title: 'AIP: ติดตามและยกเลิกพอร์ทัล'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002281"
- "5519"
ms.openlocfilehash: af2deff6b1ac8531fca9020277265f1d9d958775
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663172"
---
# <a name="aip-track-and-revoke-portal"></a><span data-ttu-id="b071f-102">AIP: ติดตามและยกเลิกพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="b071f-102">AIP: Track and revoke portal</span></span>

<span data-ttu-id="b071f-103">ใช้ **ไซต์การติดตามเอกสาร** ในพอร์ทัล Azure เพื่อติดตามและยกเลิกเอกสารเมื่อใช้การป้องกันข้อมูลของ azure</span><span class="sxs-lookup"><span data-stu-id="b071f-103">Use the **document tracking site** in the Azure Portal to track and revoke documents when using Azure Information Protection.</span></span> <span data-ttu-id="b071f-104">แอปพลิเคชัน Office (Word, Excel และ PowerPoint) และ File Explorer ยังสามารถใช้ในการติดตามและยกเลิกเอกสารได้อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="b071f-104">The Office applications (Word, Excel and PowerPoint) and File Explorer can also be used to track and revoke documents.</span></span>

1. <span data-ttu-id="b071f-105">ในไซต์การติดตามเอกสารให้คลิกยก**เลิกการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="b071f-105">In the document tracking site, click **Revoke access**.</span></span> <span data-ttu-id="b071f-106">เลิกเอกสารจะเอาการเข้าถึงออกจากผู้ใช้ที่ได้รับอนุญาต เอกสารจะไม่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="b071f-106">Revoking a document removes access from authorized users; the document is not deleted.</span></span>
2. <span data-ttu-id="b071f-107">ในแอปพลิเคชัน Office ให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="b071f-107">In the Office application:</span></span>
    - <span data-ttu-id="b071f-108">เปิดเอกสารที่ได้รับการป้องกันที่คุณต้องการติดตามหรือยกเลิก</span><span class="sxs-lookup"><span data-stu-id="b071f-108">Open the protected document that you want to track or revoke.</span></span>
    - <span data-ttu-id="b071f-109">บนแท็บ**หน้าแรก**ในกลุ่ม**การป้องกัน**ให้คลิก**ป้องกัน > ติดตามและยกเลิก**</span><span class="sxs-lookup"><span data-stu-id="b071f-109">On the **Home** tab, in the **Protection** group, click **Protect > Track and Revoke**.</span></span>

- <span data-ttu-id="b071f-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการติดตามและการเลิกเอกสารให้ดูที่[ติดตามและยกเลิก](https://docs.microsoft.com/azure/information-protection/rms-client/client-track-revoke)</span><span class="sxs-lookup"><span data-stu-id="b071f-110">For additional information on tracking and revoking a document, see [Track and Revoke](https://docs.microsoft.com/azure/information-protection/rms-client/client-track-revoke).</span></span>

<span data-ttu-id="b071f-111">สำหรับข้อมูลเกี่ยวกับการใช้ PowerShell เพื่อจัดการไซต์การติดตามเอกสารการบันทึกข้อมูลให้ดูดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b071f-111">For information on using PowerShell to manage the document tracking site, logging information, see the following:</span></span>
- [<span data-ttu-id="b071f-112">คู่มือผู้ใช้: ติดตามและยกเลิกเอกสารของคุณเมื่อคุณใช้การป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="b071f-112">User Guide: Track and revoke your documents when you use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-track-revoke)
- [<span data-ttu-id="b071f-113">คู่มือสำหรับผู้ดูแลระบบ: การกำหนดค่าและการใช้การติดตามเอกสารสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="b071f-113">Admin Guide: Configuring and using document tracking for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-document-tracking)
- [<span data-ttu-id="b071f-114">สิทธิ์การใช้งานการจัดการสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="b071f-114">Rights Management use license</span></span>](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#rights-management-use-license)
- [<span data-ttu-id="b071f-115">รีวิวการสมัครใช้งานการป้องกันข้อมูลของ Azure และฟีเจอร์</span><span class="sxs-lookup"><span data-stu-id="b071f-115">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- [<span data-ttu-id="b071f-116">ข้อกำหนดสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="b071f-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="b071f-117">บทช่วยสอนเริ่มต้นใช้งานด่วนสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="b071f-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
