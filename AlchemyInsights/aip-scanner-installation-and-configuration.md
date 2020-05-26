---
title: 'เครื่องสแกนเนอร์ AIP: การติดตั้งและการกําหนดค่า'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358568"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="361b9-102">เครื่องสแกนเนอร์ AIP: การติดตั้งและการกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="361b9-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="361b9-103">**ในการติดตั้งเครื่องสแกน AIP ให้ทําตามคําแนะนําที่แนะนํา**:</span><span class="sxs-lookup"><span data-stu-id="361b9-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="361b9-104">ถ้าคุณกําลังปรับรุ่น และไม่ทําการติดตั้งใหม่ทั้งหมด โปรดตรวจสอบให้แน่ใจว่าคุณได้ปฏิบัติตามคําแนะนําสําหรับ[การปรับรุ่นสแกนเนอร์การป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)และสําหรับไคลเอนต์การติดฉลากแบบรวม[upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="361b9-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="361b9-105">ตรวจสอบว่าคุณปฏิบัติตาม[ข้อกําหนดของไฟร์วอลล์และการตั้งค่าโครงสร้างพื้นฐานเครือข่าย](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="361b9-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="361b9-106">ตรวจสอบว่านโยบายของคุณ[ถูกตั้งค่า](https://docs.microsoft.com/azure/information-protection/configure-policy)เป็นป้ายกํากับอัตโนมัติหรือมีป้ายกํากับเริ่มต้นในนโยบาย</span><span class="sxs-lookup"><span data-stu-id="361b9-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="361b9-107">ตรวจสอบให้แน่ใจว่า มีการกําหนดค่าชนิดแฟ้มที่เกี่ยวข้องสําหรับป้ายชื่อ/การป้องกันตามที่อธิบายไว้ใน[ชนิดแฟ้มได้รับการสนับสนุน โดยไคลเอ็นต์การป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="361b9-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="361b9-108">นอกจากนี้ ถ้าคุณต้องการเปลี่ยนลักษณะการทํางานเริ่มต้น ให้ทําตามคําแนะนําเหล่านี้:[การเปลี่ยนระดับการป้องกันเริ่มต้นของแฟ้ม](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="361b9-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="361b9-109">ตรวจสอบว่า บัญชีผู้ใช้ที่กําหนดค่าให้เรียกใช้บริการสแกนเนอร์มีสิทธิ์ในการเข้าถึงที่เก็บที่กําหนดค่าไว้ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="361b9-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="361b9-110">หากคุณยังพบปัญหาโปรดส่งออกบันทึกของสแกนเนอร์และเพิ่มไปยังตั๋วสนับสนุนของคุณ</span><span class="sxs-lookup"><span data-stu-id="361b9-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="361b9-111">**ส่งออกแฟ้มบันทึกของสแกนเนอร์การป้องกันข้อมูล Azure**</span><span class="sxs-lookup"><span data-stu-id="361b9-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="361b9-112">นําทางไปยัง %localappdata%\Microsoft\MSIP ภายใต้บริบทของผู้ใช้ที่เรียกใช้บริการสแกนเนอร์</span><span class="sxs-lookup"><span data-stu-id="361b9-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="361b9-113">ซิปเนื้อหาทั้งหมดภายใต้โฟลเดอร์ MSIP</span><span class="sxs-lookup"><span data-stu-id="361b9-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="361b9-114">บันทึกบันทึกไปยังตําแหน่งที่คุณเลือกและแนบกับคําขอบริการของคุณ</span><span class="sxs-lookup"><span data-stu-id="361b9-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="361b9-115">คุณยังสามารถใช้[การส่งออก AIPLogs - onbehalf ของ](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)</span><span class="sxs-lookup"><span data-stu-id="361b9-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="361b9-116">**สําหรับข้อมูลเพิ่มเติม โปรดดูที่**:</span><span class="sxs-lookup"><span data-stu-id="361b9-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="361b9-117">การปรับใช้สแกนเนอร์การป้องกันข้อมูล Azure โดยอัตโนมัติจัดประเภท และป้องกันแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="361b9-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="361b9-118">ระบุและใช้พารามิเตอร์โทเค็นสําหรับชุด AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="361b9-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="361b9-119">เรียกใช้รอบการค้นพบและดูรายงานสําหรับสแกนเนอร์</span><span class="sxs-lookup"><span data-stu-id="361b9-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="361b9-120">ตรวจทานเอกสารประกอบการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="361b9-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="361b9-121">ข้อกําหนดสําหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="361b9-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="361b9-122">ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="361b9-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
