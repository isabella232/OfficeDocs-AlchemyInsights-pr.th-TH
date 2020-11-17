---
title: บทบาทการจัดการข้อมูลประจำตัวที่มีสิทธิ์
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089149"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="6eaad-102">บทบาทการจัดการข้อมูลประจำตัว (PIM) ที่มีสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="6eaad-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="6eaad-103">**สิทธิ์ไม่ได้รับหลังจากเปิดใช้งานบทบาท**</span><span class="sxs-lookup"><span data-stu-id="6eaad-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="6eaad-104">เมื่อคุณเปิดใช้งานบทบาทในการจัดการข้อมูลประจำตัวของ Azure AD สิทธิ์ (PIM) การเปิดใช้งานอาจไม่ได้เผยแพร่ไปยังพอร์ทัลทั้งหมดที่จำเป็นต้องมีบทบาทที่มีสิทธิ์การใช้งานได้ทันที</span><span class="sxs-lookup"><span data-stu-id="6eaad-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="6eaad-105">ในบางครั้งแม้ว่าการเปลี่ยนแปลงจะถูกเผยแพร่เว็บแคชในพอร์ทัลอาจส่งผลให้การเปลี่ยนแปลงไม่มีผลทันที</span><span class="sxs-lookup"><span data-stu-id="6eaad-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="6eaad-106">ถ้าการเปิดใช้งานของคุณล่าช้าให้ทำตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="6eaad-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="6eaad-107">ลงชื่อออกจากพอร์ทัล Azure แล้วลงชื่อเข้าใช้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="6eaad-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="6eaad-108">เมื่อคุณเปิดใช้งานบทบาท Azure AD หรือบทบาทของ Azure resource คุณจะเห็นขั้นตอนการเปิดใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="6eaad-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="6eaad-109">เมื่อทุกขั้นตอนเสร็จสมบูรณ์แล้วคุณจะเห็นลิงก์ ' ลงชื่อออก '</span><span class="sxs-lookup"><span data-stu-id="6eaad-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="6eaad-110">คุณสามารถใช้ลิงก์นี้เพื่อลงชื่อออก การทำเช่นนี้จะแก้ปัญหาส่วนใหญ่สำหรับการหน่วงเวลาการเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="6eaad-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="6eaad-111">ใน PIM ตรวจสอบว่าคุณได้แสดงรายการเป็นสมาชิกของบทบาท</span><span class="sxs-lookup"><span data-stu-id="6eaad-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="6eaad-112">ถ้าคุณกำลังเปิดใช้งานบทบาทผู้ดูแลระบบ Exchange ตรวจสอบให้แน่ใจว่าคุณได้ลงชื่อออกแล้วลงชื่อเข้าใช้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="6eaad-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="6eaad-113">ถ้าปัญหายังคงมีอยู่ให้เปิดบัตรสนับสนุนและเพิ่มสิ่งนี้เป็นปัญหา</span><span class="sxs-lookup"><span data-stu-id="6eaad-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="6eaad-114">ถ้าคุณกำลังใช้บทบาทผู้ดูแลระบบ Exchange ของคุณในการเข้าถึงศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายให้ดูขั้นตอนถัดไป</span><span class="sxs-lookup"><span data-stu-id="6eaad-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="6eaad-115">ถ้าคุณกำลังเปิดใช้งานบทบาทในการเข้าถึงศูนย์การรักษาความปลอดภัยและการปฏิบัติตามกฎระเบียบหรือถ้าคุณกำลังเปิดใช้งานบทบาทผู้ดูแลระบบ SharePoint คุณจะได้พบกับการหน่วงเวลาการเปิดใช้งานบางส่วนจากเวลาไม่กี่นาทีจนถึงสองสามชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="6eaad-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="6eaad-116">นี่เป็นปัญหาที่ทราบแล้วและเรากำลังทำงานร่วมกับทีมเหล่านี้เพื่อแก้ไขปัญหานี้โดยเร็วที่สุดเท่าที่จะเป็นไปได้</span><span class="sxs-lookup"><span data-stu-id="6eaad-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="6eaad-117">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="6eaad-117">For more information, see:</span></span>

- [<span data-ttu-id="6eaad-118">เปิดใช้งานบทบาท Azure AD ของฉันใน PIM</span><span class="sxs-lookup"><span data-stu-id="6eaad-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="6eaad-119">เปิดใช้งานบทบาทของทรัพยากร Azure ของฉันใน PIM</span><span class="sxs-lookup"><span data-stu-id="6eaad-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="6eaad-120">**สิทธิ์จะไม่ถูกเอาออกหลังจากปิดใช้งานบทบาทหรือการเปิดใช้งานบทบาทหมดอายุ**</span><span class="sxs-lookup"><span data-stu-id="6eaad-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="6eaad-121">เมื่อคุณปิดใช้งานบทบาทในการจัดการข้อมูลประจำตัวของ Azure AD สิทธิ์หรือเมื่อช่วงเวลาการเปิดใช้งานของบทบาทหมดอายุอาจเป็นการหน่วงเวลาที่คุณยังคงสามารถเข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="6eaad-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="6eaad-122">ถ้าการปิดใช้งานของคุณมีความล่าช้าให้ทำตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="6eaad-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="6eaad-123">ถ้าคุณปิดใช้งานบทบาทผู้ดูแลระบบ Exchange หรือระยะเวลาการเปิดใช้งานของบทบาทจะหมดอายุและคุณสังเกตเห็นการหน่วงเวลาที่สำคัญก่อนที่สิทธิ์จะถูกเอาออกให้เปิดบัตรสนับสนุนและแจ้งวิศวกรฝ่ายสนับสนุนของคุณเพื่อช่วยให้คุณสามารถจัดเก็บตั๋วด้วยทีมการจัดการการเข้าถึงที่มีสิทธิ์การเข้าถึง (PAM) ภายใน Office เกี่ยวกับปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="6eaad-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="6eaad-124">ถ้าช่วงเวลาการเปิดใช้งานหมดอายุแล้วแต่คุณยังมีเซสชันของเบราว์เซอร์เปิดอยู่ให้ปิดเบราว์เซอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="6eaad-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="6eaad-125">คุณยังสามารถใช้บทบาทต่อไปได้จนกว่าคุณจะปิดเซสชันนั้น</span><span class="sxs-lookup"><span data-stu-id="6eaad-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="6eaad-126">นี่เป็นปัญหาที่ทราบแล้วและเรากำลังค้นหาการแก้ไขที่เป็นไปได้ในการยกเลิกการเพิกถอนเซสชันแต่ละครั้งเมื่อการเปิดใช้งานหมดอายุแล้ว</span><span class="sxs-lookup"><span data-stu-id="6eaad-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="6eaad-127">ถ้าการหน่วงเวลาของคุณแตกต่างจากสถานการณ์สมมติสองเหล่านี้โปรดเปิดบัตรสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="6eaad-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
