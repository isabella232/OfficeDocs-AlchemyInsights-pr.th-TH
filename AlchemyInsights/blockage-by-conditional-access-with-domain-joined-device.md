---
title: ฉันถูกบล็อกโดยการเข้าถึงตามเงื่อนไขด้วยอุปกรณ์ที่เข้าร่วมในโดเมน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038105"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="ab997-102">ฉันถูกบล็อกโดยการเข้าถึงตามเงื่อนไขด้วยอุปกรณ์ที่เข้าร่วมในโดเมน</span><span class="sxs-lookup"><span data-stu-id="ab997-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="ab997-103">**เครื่องมือที่แนะนาเป็นอย่างยิ่ง**</span><span class="sxs-lookup"><span data-stu-id="ab997-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="ab997-104">[เครื่องมือแก้ไขปัญหาการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - เครื่องมือที่จะช่วยแก้ไขปัญหาการลงทะเบียนอุปกรณ์ที่พบบ่อยที่สุด</span><span class="sxs-lookup"><span data-stu-id="ab997-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="ab997-105">[ทดสอบสคริปต์การเชื่อมต่อการลงทะเบียน](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) อุปกรณ์ - สคริปต์ที่ช่วยรับรองว่าอุปกรณ์สามารถเข้าถึงจุดสิ้นสุดการลงทะเบียนอุปกรณ์ภายใต้บัญชีระบบ</span><span class="sxs-lookup"><span data-stu-id="ab997-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="ab997-106">[สคริปต์การล้างข้อมูลอุปกรณ์ Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - สคริปต์ที่ช่วยให้คุณค้นหาและจัดการอุปกรณ์เก่าในสภาพแวดล้อมของคุณ</span><span class="sxs-lookup"><span data-stu-id="ab997-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="ab997-107">ต่อไปนี้เป็นสาเหตุทั่วไปบางประการที่การเข้าถึงตามเงื่อนไขอาจล้มเหลวอุปกรณ์ที่เข้าร่วมโดเมน (Hybrid Azure AD)</span><span class="sxs-lookup"><span data-stu-id="ab997-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="ab997-108">**ไม่มี Azure AD PRT บนอุปกรณ์** - คุณต้องตรวจสอบให้แน่ใจว่าอุปกรณ์มีโทเค็นรีเฟรชหลักของ Azure AD (PRT)</span><span class="sxs-lookup"><span data-stu-id="ab997-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="ab997-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="ab997-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="ab997-110">เมื่อต้องการตรวจสอบว่าคุณมี Azure AD PRT หรือไม่ คุณสามารถเรียกใช้สั่งบนอุปกรณ์ และตรวจสอบว่า `dsregcmd/status` "AzureAdPrt" เท่ากับ "YES" หรือไม่</span><span class="sxs-lookup"><span data-stu-id="ab997-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="ab997-111">ถ้า "AzureAdPrt" เป็น "NO" ให้ตรวจสอบดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ab997-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="ab997-112">**ไม่ว่าคุณจะ** มีสภาพแวดล้อมภายนอกกับ AD FS และไม่สามารถเข้าถึงได้จากเครือข่ายหลักของผู้ใช้ของคุณ : ในกรณีนี้ ตรวจสอบให้แน่ใจว่าจุดสิ้นสุด "usernamemixed" ของคุณสามารถเข้าถึงได้จากเอกซ์ทราเน็ต</span><span class="sxs-lookup"><span data-stu-id="ab997-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="ab997-113">ถ้า AD FS ของคุณอยู่หลัง VPN ตรวจสอบให้แน่ใจว่าผู้ใช้เชื่อมต่อกับ VPN และลงชื่อเข้าใช้อุปกรณ์อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="ab997-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="ab997-114">ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)นี้</span><span class="sxs-lookup"><span data-stu-id="ab997-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="ab997-115">**TPM ของอุปกรณ์** เป็นข้อผิดพลาดหรือไม่ และไม่สามารถรับรองความถูกต้องของอุปกรณ์ได้ : ตรวจสอบ "tpm.msc" เพื่อดูว่าสถานะของ TPM เป็น "พร้อมแล้ว" หรือไม่</span><span class="sxs-lookup"><span data-stu-id="ab997-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="ab997-116">ถ้าไม่ ให้ `dsregcmd/leave` เรียกใช้และให้อุปกรณ์เข้าร่วมกับ Azure AD อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="ab997-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="ab997-117">จากนั้นลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="ab997-117">Then, try again.</span></span> <span data-ttu-id="ab997-118">ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)นี้</span><span class="sxs-lookup"><span data-stu-id="ab997-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="ab997-119">**คุณใช้งานผู้ให้บริการข้อมูลเฉพาะตัวของบริษัทอื่น ซึ่งไม่สนับสนุนWS-Trustโพรโทคอล**</span><span class="sxs-lookup"><span data-stu-id="ab997-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="ab997-120">ตามที่อธิบายไว้ในเอกสารของเรา อุปกรณ์ที่เข้าร่วม Azure AD แบบไฮบริดจะไม่สามารถใช้งานในกรณีนี้ได้</span><span class="sxs-lookup"><span data-stu-id="ab997-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="ab997-121">โปรดติดต่อผู้ให้บริการข้อมูลเฉพาะตัวของคุณเพื่อรับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="ab997-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="ab997-122">ผู้ใช้ใช้เบราว์เซอร์ Chrome โดยไม่มีบัญชี **Windows 10** หรือ Chrome ส่วนขยาย Office จะไม่ใช้ PRT บนอุปกรณ์ที่เข้าร่วม **ด้วย AAD** หรืออุปกรณ์ที่เข้าร่วมแบบไฮบริดโดยอัตโนมัติ: ซึ่งไปสู่ความล้มเหลวในการนโยบายการเข้าถึงตามเงื่อนไขบนอุปกรณ์ใดๆ ที่มีข้อความแสดงข้อผิดพลาด "อุปกรณ์ที่ไม่ได้ลงทะเบียน" แสดงขึ้น</span><span class="sxs-lookup"><span data-stu-id="ab997-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="ab997-123">เมื่อต้องการใช้เบราว์เซอร์ Chrome อย่างถูกต้อง คุณต้องติดตั้ง "บัญชี Windows 10" หรือ "ส่วนขยาย Office ไปยังเบราว์เซอร์ Chrome ของผู้ใช้" ผ่าน SCCM หรือ Intun e</span><span class="sxs-lookup"><span data-stu-id="ab997-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="ab997-124">ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)นี้</span><span class="sxs-lookup"><span data-stu-id="ab997-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="ab997-125">ถ้าไม่สามารถส่งส่วนขยายระยะไกลได้ ให้แจ้งให้ผู้ใช้ติดตั้งส่วนขยายข้างต้นด้วยตนเองเพื่อเข้าถึงแอปพลิเคชันที่อยู่เบื้องหลังการเข้าถึงตามเงื่อนไขบนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="ab997-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="ab997-126">ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)นี้</span><span class="sxs-lookup"><span data-stu-id="ab997-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="ab997-127">อุปกรณ์ถูกรวม Azure AD แบบไฮบริดอย่างถูกต้อง แต่ถูกลบหรือปิดใช้งานโดยไม่ได้ตั้งใจ ไม่ว่าจะเกิดจากการซิงค์การเปลี่ยนแปลงใน **Azure AD Connect** หรือจากพอร์ทัล Azure : ในกรณีนี้ วัตถุอุปกรณ์จะไม่ถูกรับรู้ว่าเป็นอุปกรณ์ที่เข้าร่วมโดยสมบูรณ์อีกต่อไป แม้ว่าสถานะ "AzureAdJoined" และ "PRT" จะแสดงอย่างถูกต้องบนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="ab997-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="ab997-128">เมื่อต้องการแก้ไขปัญหานี้ ให้เรียกใช้ `dsregcmd/leave` บนอุปกรณ์ที่ได้รับผลกระทบและให้พวกเขาเข้าร่วม Azure AD อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="ab997-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="ab997-129">ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)นี้</span><span class="sxs-lookup"><span data-stu-id="ab997-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="ab997-130">ถ้าอุปกรณ์ของคุณอยู่ในการอัปเดต Windows 10, 1809 ด้วยพร็อกซี VPN/Cloud และดูปัญหาเกี่ยวกับ "AzureAdPrt" หรือแอปใดๆ ที่มีปัญหา SSO (Outlook ไม่ได้เชื่อมต่อกับกล่องจดหมายแม้ว่าคุณจะมี PRT) ตรวจสอบให้แน่ใจว่าคุณมีโปรแกรมแก้ไข [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) หรือการอัปเดตสะสมในเดือนเมษายน [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) เพื่อป้องกันการ PRT ล้มเหลวบนเครื่องเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="ab997-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















