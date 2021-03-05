---
title: การกําหนดค่าบริการการซิงค์ MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482895"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="63ac5-102">การกําหนดค่าบริการการซิงค์ MIM</span><span class="sxs-lookup"><span data-stu-id="63ac5-102">Configure MIM Sync service</span></span>

<span data-ttu-id="63ac5-103">บริการการซิงโครไนซ์ Microsoft Identity Manager (MIM) เป็นคอมโพเนนต์ของ MIM</span><span class="sxs-lookup"><span data-stu-id="63ac5-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="63ac5-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span><span class="sxs-lookup"><span data-stu-id="63ac5-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="63ac5-105">คุณอาจสามารถแก้ไขปัญหาของคุณด้วยการซิงค์ MIM ถ้าปัญหาได้รับการแก้ไขในการอัปเดตล่าสุดเป็น MIM หรือเป็นหนึ่งในปัญหาอื่นๆ ที่กล่าวถึงในส่วนด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="63ac5-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="63ac5-106">**ขั้นตอนที่แนะนา**</span><span class="sxs-lookup"><span data-stu-id="63ac5-106">**Recommended steps**</span></span>

1. <span data-ttu-id="63ac5-107">ตรวจสอบให้แน่ใจว่าคุณได้ใช้การอัปเดตล่าสุดของการซิงค์ MIM และตรวจสอบบันทึกย่อการเปิดตัวการซิงค์ [MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) เพื่อตรวจสอบว่าปัญหาได้รับการแก้ไขในการอัปเดตหรือไม่</span><span class="sxs-lookup"><span data-stu-id="63ac5-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="63ac5-108">ถ้าปัญหาอยู่กับทั่วไป LDAP, Generic SQL, Lotus Domino หรือตัวเชื่อมต่อบริการเว็บ ตรวจสอบให้แน่ใจว่าคุณใช้การอัปเดตล่าสุดของ [ตัวเชื่อมต่อ](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="63ac5-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="63ac5-109">ถ้าการซิงค์ MIM หยุดที่มีข้อผิดพลาด ให้ดูตารางรหัสข้อผิดพลาด [การเรียกใช้](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) เพื่อระบุสาเหตุที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="63ac5-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="63ac5-110">ถ้าการเรียกใช้หยุดโดยมีข้อยกเว้นส่วนขยาย **dll** ให้คลิกที่ข้อความเหล่านั้นเพื่อเปิดหน้าต่างคุณสมบัติวัตถุ Space **Connector** แล้วคลิกที่ **Stack Trace...** เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับสาเหตุพื้นฐาน ตามที่อธิบายไว้ในข้อยกเว้นส่วนขยาย [-DLL](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)</span><span class="sxs-lookup"><span data-stu-id="63ac5-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="63ac5-111">ถ้าคอมโพเนนต์ของบริการการแจ้งให้ทราบการเปลี่ยนแปลงรหัสผ่าน (PCNS) รายงานข้อผิดพลาด **6025** ในบันทึกเหตุการณ์ระหว่างการซิงโครไนซ์รหัสผ่าน ให้ตรวจสอบคู่มือการแก้ไขปัญหาข้อผิดพลาดการรายงาน [PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)</span><span class="sxs-lookup"><span data-stu-id="63ac5-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="63ac5-112">ถ้าการซิงโครไนซ์กับตัวแทนการจัดการบริการ FIM ช้า ให้ตรวจสอบการตั้งค่าเพิ่มโดยอัตโนมัติของ TempDB ตามที่อธิบายไว้ใน การแก้ไขปัญหาช้าหรือหยุดการตอบสนอง[การซิงโครไนซ์](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="63ac5-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="63ac5-113">ถ้าคุณพบข้อผิดพลาดของเซิร์ฟเวอร์ที่หยุดเมื่อเกิดข้อผิดพลาดในการสร้างผ่านบริการเว็บโดยใช้ตัวแทนการจัดการบริการ FIM ให้ดูข้อมูลสนับสนุน: การสร้างล้มเหลวผ่าน [บริการ](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) เว็บเพื่อดูภาพรวมของสาเหตุ</span><span class="sxs-lookup"><span data-stu-id="63ac5-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

