---
title: การซิงโครไนซ์รหัสผ่าน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483086"
---
# <a name="password-synchronization"></a><span data-ttu-id="513f1-102">การซิงโครไนซ์รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="513f1-102">Password synchronization</span></span>

<span data-ttu-id="513f1-103">**การซิงโครไนซ์แฮชของรหัสผ่านไม่สมบูรณ์**</span><span class="sxs-lookup"><span data-stu-id="513f1-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="513f1-104">ปัญหาทั่วไปที่ลูกค้าพบเมื่อการซิงโครไนซ์แฮชของรหัสผ่านใช้งานไม่ได้:</span><span class="sxs-lookup"><span data-stu-id="513f1-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="513f1-105">บัญชี Active Directory ที่ใช้โดย Azure AD Connect เพื่อสื่อสารกับ Active Directory ภายในองค์กรจะไม่ได้รับอนุญาตให้ **Replicate Directory Changes** และ **Replicate Directory Changes** All ซึ่งต้องใช้ในการซิงโครไนซ์รหัสผ่าน คุณจึงต้องแก้ไขปัญหานี้โดยให้สิทธิ์เหล่านี้กับบัญชี Active Directory</span><span class="sxs-lookup"><span data-stu-id="513f1-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="513f1-106">การซิงโครไนซ์แฮชรหัสผ่านจะถูกปิดใช้งานหลังจากผู้ดูแลระบบเปลี่ยนวิธี Sign-In ผู้ใช้จากการซิงโครไนซ์รหัสผ่านเป็นตัวเลือกอื่น เช่น การติดต่อกับภายนอกด้วย **AD FS** ในตัวช่วยสร้าง Azure AD Connect - คุณสามารถแก้ไขปัญหานี้ได้โดยการเปิดใช้งานฟีเจอร์การซิงโครไนซ์แฮชของรหัสผ่านอีกครั้งในตัวช่วยสร้าง Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="513f1-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="513f1-107">ปัญหาการเชื่อมต่อกับ Active Directory ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="513f1-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="513f1-108">ตัวอย่างเช่น บางตัวควบคุมโดเมนไม่สามารถเข้าถึงได้โดย Azure AD Connect หรือพอร์ตที่ต้องมีถูก[](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)บล็อกโดยไฟร์วอลล์ คุณจึงต้องแก้ไขปัญหานี้โดยการตรวจสอบให้แน่ใจว่าการเชื่อมต่อระหว่างเซิร์ฟเวอร์ Azure AD Connect และ Active Directory ภายในองค์กรสามารถใช้งานได้อย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="513f1-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="513f1-109">เซิร์ฟเวอร์ Azure AD Connect ที่อยู่ในโหมดการจัดเตรียมอยู่ในขณะนี้ ซึ่งจะส่งผลให้เซิร์ฟเวอร์ไม่สามารถไปที่ Hashes ของรหัสผ่านได้ - เมื่อต้องการแก้ไขปัญหา ให้ปฏิบัติตามขั้นตอนที่อธิบายไว้ในส่วนแก้ไขปัญหาการซิงโครไนซ์รหัสผ่านด้วย [การซิงค์ Azure AD Connect -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)ไม่มีการซิงโครไนซ์รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="513f1-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="513f1-110">**การซิงโครไนซ์แฮชของรหัสผ่านไม่ใช้งานกับผู้ใช้บางรายของฉัน**</span><span class="sxs-lookup"><span data-stu-id="513f1-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="513f1-111">ถ้าคุณสังเกตเห็นว่าแฮชของรหัสผ่านไม่ซิงค์กับผู้ใช้ ให้ใช้งาน **แก้ไขปัญหา** ใน Azure AD Connect เพื่อตรวจสอบและแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="513f1-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="513f1-112">ให้ดการงานต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="513f1-112">Perform the following tasks:</span></span>

    <span data-ttu-id="513f1-113">a.</span><span class="sxs-lookup"><span data-stu-id="513f1-113">a.</span></span> [<span data-ttu-id="513f1-114">เรียกใช้งานการแก้ไขปัญหาในตัวช่วยสร้าง</span><span class="sxs-lookup"><span data-stu-id="513f1-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="513f1-115">b.</span><span class="sxs-lookup"><span data-stu-id="513f1-115">b.</span></span> [<span data-ttu-id="513f1-116">ใช้ cmdlet การแก้ไขปัญหาเพื่อตรวจสอบปัญหาการซิงค์แฮชรหัสผ่านในการใช้งานเฉพาะ</span><span class="sxs-lookup"><span data-stu-id="513f1-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="513f1-117">วัตถุผู้ใช้ Active Directory ภายในองค์กรถูกเปิดใช้งานไว้ **เพื่อให้ผู้ใช้ต้องเปลี่ยนรหัสผ่านที่ตัวเลือกการเข้าสู่ระบบ** ถัดไป</span><span class="sxs-lookup"><span data-stu-id="513f1-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="513f1-118">เมื่อเปิดใช้งานตัวเลือกนี้ ผู้ใช้จะถูกมอบหมายรหัสผ่านชั่วคราวและจะได้รับพร้อมท์ให้เปลี่ยนรหัสผ่านบนการเข้าสู่ระบบครั้งถัดไป</span><span class="sxs-lookup"><span data-stu-id="513f1-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="513f1-119">Azure AD Connect ไม่ซิงโครไนซ์รหัสผ่านชั่วคราวกับ Azure AD</span><span class="sxs-lookup"><span data-stu-id="513f1-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="513f1-120">เมื่อต้องการแก้ไขปัญหาข้างต้น ให้ปฏิบัติอย่างใดอย่างหนึ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="513f1-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="513f1-121">ขอให้ผู้ใช้ลงชื่อเข้าใช้แอปพลิเคชันภายในองค์กร (ตัวอย่างเช่น เดสก์ท็อป Windows) และเปลี่ยนรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="513f1-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="513f1-122">รหัสผ่านใหม่จะถูกซิงโครไนซ์กับ Azure AD</span><span class="sxs-lookup"><span data-stu-id="513f1-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="513f1-123">ให้ผู้ดูแลระบบอัปเดตรหัสผ่านของผู้ใช้โดยไม่เปิดใช้งานตัวเลือก ที่ผู้ใช้ต้องเปลี่ยนรหัสผ่าน **ในการเข้าสู่ระบบ** ครั้งถัดไป และแชร์รหัสผ่านใหม่กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="513f1-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="513f1-124">วัตถุผู้ใช้ Active Directory ภายในองค์กรไม่ได้ถูก **กําหนดค่าอย่างถูกต้องในการ** ซิงโครไนซ์วัตถุหรือการซิงโครไนซ์รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="513f1-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="513f1-125">เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนที่อธิบายไว้ในการซิงโครไนซ์แฮช[ของรหัสผ่านการแก้ไขปัญหาด้วยการซิงค์ Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="513f1-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







