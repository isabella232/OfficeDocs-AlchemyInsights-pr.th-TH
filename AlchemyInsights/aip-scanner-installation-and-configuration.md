---
title: 'ตัวสแกน AIP: การติดตั้งและการกําหนดค่า'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821682"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="c58c7-102">ตัวสแกน AIP: การติดตั้งและการกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="c58c7-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="c58c7-103">**เมื่อต้องการติดตั้งสแกนเนอร์ AIP ให้ปฏิบัติตามแนวทางที่แนะนํา**:</span><span class="sxs-lookup"><span data-stu-id="c58c7-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="c58c7-104">ถ้าคุณอัปเกรดและไม่ได้ติดตั้งใหม่ทั้งหมด โปรดตรวจสอบให้แน่ใจว่าคุณได้ปฏิบัติตามแนวทางการอัปเกรดตัวสแกน Azure Information [Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)และไคลเอ็นต์การลงป้ายแบบรวมศูนย์ ให้ดู การอัปเกรดตัวสแกน[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="c58c7-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="c58c7-105">ตรวจสอบว่าคุณปฏิบัติตามข้อกฎหมาย [การตั้งค่าไฟร์วอลล์และโครงสร้างพื้นฐานของเครือข่าย](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="c58c7-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="c58c7-106">ตรวจสอบให้แน่ใจว่า [นโยบายของคุณถูกตั้งค่า](https://docs.microsoft.com/azure/information-protection/configure-policy) ให้ติดป้ายผนึกอัตโนมัติหรือมีป้ายชื่อเริ่มต้นในนโยบาย</span><span class="sxs-lookup"><span data-stu-id="c58c7-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="c58c7-107">ตรวจสอบให้แน่ใจว่าชนิดไฟล์ที่เกี่ยวข้องได้รับการกําหนดค่าไว้ป้ายชื่อ/การป้องกันตามที่อธิบายไว้[ใน ชนิดไฟล์ ที่สนับสนุนโดยไคลเอ็นต์ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="c58c7-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="c58c7-108">นอกจากนี้ ถ้าคุณต้องการเปลี่ยนลักษณะการรักษาความปลอดภัยเริ่มต้น ให้ปฏิบัติตามแนวทาง [เหล่านี้: การเปลี่ยนระดับการป้องกันเริ่มต้นของ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)ไฟล์</span><span class="sxs-lookup"><span data-stu-id="c58c7-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="c58c7-109">ตรวจสอบว่าบัญชีผู้ใช้ที่กําหนดค่าให้เรียกใช้บริการสแกนเนอร์มีสิทธิ์ในการเข้าถึงที่เก็บที่กําหนดค่าไว้ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="c58c7-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="c58c7-110">ถ้าคุณยังคงพบปัญหา โปรดส่งออกบันทึกสแกนเนอร์และเพิ่มบันทึกลงในตั๋วการสนับสนุนของคุณ</span><span class="sxs-lookup"><span data-stu-id="c58c7-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="c58c7-111">**ส่งออกบันทึก Azure Information Protection Scanner**</span><span class="sxs-lookup"><span data-stu-id="c58c7-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="c58c7-112">นําทางไปยัง %localappdata%\Microsoft\MSIP ภายใต้บริบทของผู้ใช้ที่เรียกใช้บริการสแกนเนอร์</span><span class="sxs-lookup"><span data-stu-id="c58c7-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="c58c7-113">Zip เนื้อหาทั้งหมดภายใต้โฟลเดอร์ MSIP</span><span class="sxs-lookup"><span data-stu-id="c58c7-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="c58c7-114">บันทึกแฟ้มบันทึกไปยังตัวเลือกของสถานที่และแนบไฟล์กับการร้องขอบริการของคุณ</span><span class="sxs-lookup"><span data-stu-id="c58c7-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="c58c7-115">คุณยังสามารถใช้[Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)</span><span class="sxs-lookup"><span data-stu-id="c58c7-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="c58c7-116">**หากต้องการข้อมูลเพิ่มเติม โปรดดู**:</span><span class="sxs-lookup"><span data-stu-id="c58c7-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="c58c7-117">การปรับใช้ตัวสแกน Azure Information Protection เพื่อจัดประเภทและปกป้องไฟล์โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="c58c7-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="c58c7-118">ระบุและใช้พารามิเตอร์โทเค็นใน Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="c58c7-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="c58c7-119">เรียกใช้รอบการค้นพบและดูรายงานของสแกนเนอร์</span><span class="sxs-lookup"><span data-stu-id="c58c7-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="c58c7-120">ตรวจทานเอกสาร Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c58c7-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="c58c7-121">ความต้องการของ Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c58c7-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="c58c7-122">ดาวน์โหลดไคลเอ็นต์ Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c58c7-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
