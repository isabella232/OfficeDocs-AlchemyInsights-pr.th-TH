---
title: 646วิธีการกําหนดค่า AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722582"
---
# <a name="configure-sync-features"></a><span data-ttu-id="18e81-102">กําหนดค่าคุณลักษณะการซิงค์</span><span class="sxs-lookup"><span data-stu-id="18e81-102">Configure sync features</span></span>

<span data-ttu-id="18e81-103">การเชื่อมต่อ AD Azure มีคุณลักษณะหลายอย่างที่เปิดใช้งาน โดยค่าเริ่มต้น หรือที่คุณสามารถเปิดใช้งานในภายหลัง</span><span class="sxs-lookup"><span data-stu-id="18e81-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="18e81-104">คุณลักษณะบางอย่างจําเป็นต้องมีการกําหนดค่าเพิ่มเติมในสภาพแวดล้อมเฉพาะ</span><span class="sxs-lookup"><span data-stu-id="18e81-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="18e81-105">[การกรอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)จํากัดวัตถุจะซิงโครไนส์กับโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="18e81-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="18e81-106">โดยค่าเริ่มต้น ผู้ใช้ทั้งหมด ผู้ติดต่อ กลุ่ม และ Windows 10 บัญชีคอมพิวเตอร์จะซิงโครไนส์</span><span class="sxs-lookup"><span data-stu-id="18e81-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="18e81-107">คุณสามารถรวมหรือแยกวัตถุตามโดเมน, OUs หรือแอตทริบิวต์อื่นๆ ได้</span><span class="sxs-lookup"><span data-stu-id="18e81-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="18e81-108">[ซิงโครไนส์แฮรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)แฮซิงโครไนส์แฮรหัสผ่านจากไดเรกทอรีที่ใช้งานอยู่ในสถานที่เพื่อโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="18e81-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="18e81-109">วิธีนี้ช่วยให้การจัดการรหัสผ่านอยู่ในตําแหน่งเดียว แต่ใช้รหัสผ่านเดียวกันทั้งในสภาพแวดล้อมภายในและระบบคลาวด์</span><span class="sxs-lookup"><span data-stu-id="18e81-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="18e81-110">เนื่องจาก Active Directory เป็นแหล่งที่เชื่อถือได้ คุณจึงสามารถใช้นโยบายรหัสผ่านของคุณเองได้</span><span class="sxs-lookup"><span data-stu-id="18e81-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="18e81-111">[การรีเซ็ตรหัสผ่านด้วยตนเอง (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)ช่วยให้ผู้ใช้สามารถรีเซ็ตรหัสผ่านของตนเองในระบบคลาวด์ในขณะที่ยังคงใช้นโยบายรหัสผ่านในสถานที่ของคุณ</span><span class="sxs-lookup"><span data-stu-id="18e81-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="18e81-112">[อุปกรณ์ writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)ช่วยให้อุปกรณ์ที่ลงทะเบียนในโฆษณา Azure จะถูกเขียนกลับไปยังไดเรกทอรีที่ใช้งานอยู่ในสถานที่เพื่อให้สามารถใช้สําหรับการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="18e81-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="18e81-113">[ป้องกันการลบโดยไม่ตั้งใจ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)ถูกเปิดใช้งานโดยค่าเริ่มต้นเพื่อช่วยป้องกันการลบวัตถุพร้อมกันมากเกินไป (มากกว่า 500 วัตถุต่อการทําข้อมูลให้ตรงกัน)</span><span class="sxs-lookup"><span data-stu-id="18e81-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="18e81-114">คุณสามารถเปลี่ยนการตั้งค่านี้ให้ตรงกับความต้องการขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="18e81-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="18e81-115">[การปรับรุ่นอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)ถูกเปิดใช้งานโดยค่าเริ่มต้นสําหรับการติดตั้งแบบด่วน และช่วยให้มั่นใจว่ารุ่นของการเชื่อมต่อ AD Azure เป็นรุ่นล่าสุดอยู่เสมอ</span><span class="sxs-lookup"><span data-stu-id="18e81-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
