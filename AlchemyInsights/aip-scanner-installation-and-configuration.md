---
title: 'การสแกน AIP: การติดตั้งและการกำหนดค่า'
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
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686661"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="26b20-102">การสแกน AIP: การติดตั้งและการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="26b20-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="26b20-103">**เมื่อต้องการติดตั้งสแกนเนอร์ AIP ให้ทำตามแนวทางที่แนะนำ**:</span><span class="sxs-lookup"><span data-stu-id="26b20-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="26b20-104">ถ้าคุณกำลังอัปเกรดและไม่ได้ทำการติดตั้งใหม่ทั้งหมดโปรดตรวจสอบให้แน่ใจว่าคุณได้ทำตามแนวทางสำหรับการ[อัปเกรดสแกนเนอร์การป้องกันข้อมูลของ azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)และสำหรับไคลเอ็นต์การติดฉลากแบบรวมให้ดู[ที่การอัปเกรดสแกนเนอร์การป้องกันข้อมูลของ azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="26b20-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="26b20-105">ตรวจสอบว่าคุณสอดคล้องกับ [ไฟร์วอลล์และความต้องการตั้งค่าโครงสร้างพื้นฐานของเครือข่าย](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="26b20-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="26b20-106">ตรวจสอบให้แน่ใจว่านโยบายของคุณ [ถูกตั้งค่า](https://docs.microsoft.com/azure/information-protection/configure-policy) เป็นการติดฉลากอัตโนมัติหรือมีป้ายชื่อเริ่มต้นในนโยบาย</span><span class="sxs-lookup"><span data-stu-id="26b20-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="26b20-107">ตรวจสอบให้แน่ใจว่าชนิดไฟล์ที่เกี่ยวข้องถูกกำหนดค่าสำหรับป้ายชื่อ/การป้องกันตามที่อธิบายไว้ใน[ชนิดไฟล์ที่ได้รับการสนับสนุนโดยไคลเอ็นต์การป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="26b20-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="26b20-108">นอกจากนี้ถ้าคุณต้องการเปลี่ยนลักษณะการทำงานเริ่มต้นให้ทำตามแนวทางเหล่านี้:[การเปลี่ยนระดับการป้องกันเริ่มต้นของไฟล์](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="26b20-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="26b20-109">ตรวจสอบว่าบัญชีผู้ใช้ที่ได้รับการกำหนดค่าให้เรียกใช้บริการสแกนเนอร์มีสิทธิ์ในการเข้าถึงที่เก็บที่กำหนดค่าไว้ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="26b20-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="26b20-110">ถ้าคุณยังคงประสบปัญหาโปรดส่งออกบันทึกของสแกนเนอร์และเพิ่มไฟล์เหล่านั้นลงในตั๋วสนับสนุนของคุณ</span><span class="sxs-lookup"><span data-stu-id="26b20-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="26b20-111">**ส่งออกบันทึกสแกนเนอร์การป้องกันข้อมูล Azure**</span><span class="sxs-lookup"><span data-stu-id="26b20-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="26b20-112">นำทางไปยัง%localappdata%\Microsoft\MSIP ภายใต้บริบทของผู้ใช้ที่กำลังเรียกใช้บริการสแกนเนอร์</span><span class="sxs-lookup"><span data-stu-id="26b20-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="26b20-113">Zip เนื้อหาทั้งหมดภายใต้โฟลเดอร์ MSIP</span><span class="sxs-lookup"><span data-stu-id="26b20-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="26b20-114">บันทึกไฟล์บันทึกไปยังตำแหน่งที่ตั้งของคุณและแนบเข้ากับคำขอบริการของคุณ</span><span class="sxs-lookup"><span data-stu-id="26b20-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="26b20-115">นอกจากนี้คุณยังสามารถใช้การ[ส่งออก-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)</span><span class="sxs-lookup"><span data-stu-id="26b20-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="26b20-116">**สำหรับข้อมูลเพิ่มเติมให้ดู**ที่:</span><span class="sxs-lookup"><span data-stu-id="26b20-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="26b20-117">การปรับใช้สแกนเนอร์การป้องกันข้อมูลของ Azure เพื่อจัดประเภทและป้องกันไฟล์โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="26b20-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="26b20-118">ระบุและใช้พารามิเตอร์โทเค็นสำหรับการตั้งค่า-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="26b20-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="26b20-119">การเรียกใช้วงจรการค้นหาและดูรายงานสำหรับสแกนเนอร์</span><span class="sxs-lookup"><span data-stu-id="26b20-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="26b20-120">ตรวจทานเอกสารประกอบการป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="26b20-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="26b20-121">ข้อกำหนดสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="26b20-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="26b20-122">ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="26b20-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
