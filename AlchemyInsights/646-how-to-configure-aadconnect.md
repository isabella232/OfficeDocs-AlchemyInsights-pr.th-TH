---
title: 646 วิธีการการตั้งค่าคอนฟิก AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: dd6d6986b23c8adcc98fe713bacf32fb5bf8b4b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915607"
---
# <a name="configure-sync-features"></a><span data-ttu-id="ba2c2-102">การตั้งค่าคอนฟิกลักษณะการทำข้อมูลให้ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="ba2c2-102">Configure sync features</span></span>

<span data-ttu-id="ba2c2-p101">การเชื่อมต่อ AD azure มีคุณลักษณะหลายประการที่จะเปิดใช้งาน โดยค่าเริ่มต้น หรือ ที่คุณสามารถเปิดใช้งานในภายหลัง คุณลักษณะบางอย่างจำเป็นต้องมีการตั้งค่าคอนฟิกเพิ่มเติมในสภาพแวดล้อมที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="ba2c2-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="ba2c2-p102">ขีดจำกัด[การกรอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)วัตถุจะซิงโครไนส์เพื่อโฆษณา Azure โดยค่าเริ่มต้น ผู้ใช้ ผู้ติดต่อ กลุ่ม และทั้งหมด Windows 10 บัญชีคอมพิวเตอร์มีการซิงโครไนส์ คุณสามารถรวม หรือไม่รวมวัตถุที่ยึดตามโดเมน Ou หรือแอททริบิวต์อื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="ba2c2-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="ba2c2-p103">[Syncronization แฮชของรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)ซิงโครไนส์แฮชของรหัสผ่านจากไดเรกทอรีที่ใช้งานอยู่ในสถานที่เพื่อโฆษณา Azure ซึ่งช่วยให้การจัดการรหัสผ่านในสถานหนึ่ง แต่ใช้รหัสผ่านเดียวกันในทั้งสองในสถาน และสภาพแวดล้อมที่ cloud เนื่องจากไดเรกทอรีที่ใช้งานอยู่ไม่เชื่อถือแหล่งที่มา คุณสามารถใช้นโยบายรหัสผ่านของคุณเอง</span><span class="sxs-lookup"><span data-stu-id="ba2c2-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="ba2c2-111">[(SSPR) การรีเซ็ตรหัสผ่านด้วยตนเอง](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)อนุญาตให้ผู้ใช้สามารถรีเซ็ตรหัสผ่านของตนเองใน cloud ขณะที่ยังคง ใช้นโยบายรหัสผ่านของคุณในสถาน</span><span class="sxs-lookup"><span data-stu-id="ba2c2-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="ba2c2-112">[เขียนกลับอุปกรณ์](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)ช่วยให้อุปกรณ์ที่ลงทะเบียนใน Azure โฆษณาที่มีการบันทึกกลับไปยัง Active Directory ในสถานเพื่อให้สามารถใช้สำหรับการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="ba2c2-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="ba2c2-p104">[กรณีการป้องกันลบ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)ถูกเปิดใช้งาน โดยค่าเริ่มต้นเพื่อช่วยป้องกันการลบวัตถุพร้อม ๆ กันมากเกินไป (เกินกว่า 500 วัตถุต่อการซิงโครไนส์) คุณสามารถเปลี่ยนการตั้งค่านี้ให้ตรงกับความต้องการขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="ba2c2-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="ba2c2-115">[การอัพเกรดอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)ถูกเปิดใช้งาน โดยค่าเริ่มต้นสำหรับการติดตั้งด่วน และช่วยให้แน่ใจว่า เชื่อมต่อ AD Azure รุ่นของคุณเป็นปัจจุบันเสมอ</span><span class="sxs-lookup"><span data-stu-id="ba2c2-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

