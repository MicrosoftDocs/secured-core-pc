---
title: Windows 10 Secured-core PCs overview
description: This document provides an overview of the Windows 10 Secured-core PCs and Baseline Windows security for device purchase decision makers. 
ms.date: 08/18/2020
ms.topic: article
ms.author: bkendall
---

# Windows 10 Secured-core PCs

Microsoft works closely with OEM partners to help ensure that all certified Windows systems deliver a secure operating environment.  Windows integrates closely with the hardware to deliver protections that take advantage of available hardware capabilities:

- Baseline Windows security – recommended baseline for all individual systems that provides foundational system integrity protections. Leverages TPM 2.0 for a hardware root of trust, secure boot and BitLocker drive encryption.
- Virtualization-based security enabled – leverages virtualization capabilities from hardware and the hypervisor to provide additional protection for critical subsystems and data.
- Secured-core – recommended for the most sensitive systems and industries like financial, healthcare, and government agencies. Builds on the previous layers and leverages advanced processor capabilities to provide protection from firmware attacks.

## Secured-core PCs

Microsoft is working closely with OEM partners and silicon vendors to build Secured-core PCs that features deeply integrated hardware, firmware and software to ensure enhanced security for devices, identities and data.

Secured-core PCs provide protections that are useful against sophisticated attacks and can provide increased assurance when handling mission-critical data in some of the most data-sensitive industries, such as healthcare workers that handle medical records and other personally identifiable information (PII), commercial roles that handle high business impact and highly sensitive data, such as a financial controller with earnings data.

For general purpose laptops, tablets, 2-in-1’s, mobile workstations, and desktops, Microsoft recommends using Security baselines for optimal configuration. For more info, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines).

Baseline Windows security is supported by Secure Boot, Bitlocker device encryption, Windows Defender, Windows Hello and a TPM 2.0 chip to provide a hardware root of trust for the OS platform. These features are designed to secure general purpose modern devices. If you are a decision maker purchasing new devices, your devices should meet the baseline Windows security requirements.

In addition, Windows 10 in S mode provides an additional layer of security with flexibility. S mode is a configuration that’s available on all Windows editions. By ensuring only trusted applications are run on the system, S mode keeps the Windows experience fast and secured. This comes with some cost in terms of compatibility, but Intune also allows customers to install applications on an S mode system, while maintaining the S mode protections against running non-trusted applications.

## What makes a Secured-core PC

<table>
<thead>
  <tr>
    <th>Benefit </th>
    <th>Feature</th>
    <th>Hardware/Firmware requirement</th>
    <th>Baseline Windows Security</th>
    <th>Secured-core PCs</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td rowspan=5>Create a hardware backed root of trust</td>
    <td>Trusted Platform Module 2.0 (TPM)</td>
    <td>Meet the latest Microsoft requirements for the Trusted Computing Group (TCG) specification</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>Dynamic Root of Trust for Measurement (DRTM)</td>
    <td>Enabled on device (via Secure Launch)</td>
    <td></td>
    <td>V</td>
  </tr>
  <tr>
    <td>System Management Mode (SMM)</td>
    <td>Enabled on device (via System Guard)</td>
    <td></td>
    <td>V</td>
  </tr>
  <tr>
    <td>Secure Boot</td>
    <td>Secure Boot is enabled in the BIOS by default.</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>Memory Access Protection</td>
    <td>The device supports Memory Access Protection (Kernel DMA Protection)</td>
    <td></td>
    <td>V</td>
  </tr>
  <tr>
    <td>Ensure strong code integrity</td>
    <td>Hypervisor Code Integrity (HVCI)</td>
    <td>Enabled on device</td>
    <td></td>
    <td>V</td>
  </tr>
  <tr>
    <td>Provide advanced identity verification and protection</td>
    <td>Windows Hello</td>
    <td>If device supports Windows Hello, then those implementations must be capable of Enhanced sign-in.  “Capable” means:
        <ul>
            <li>Designed-in SecureBIO capable components for the Windows Hello modes are supported on the device (Face and/or Fingerprint)</li>
            <li>The device has the right SecureBIO components to enable SecureBIO functionality in a future OS release; meaning, the device BIOS implements the necessary SecureBIO SDEV table, but it is disabled by DEFAULT until supported by a future OS version.</li>
        </ul>
    </td>
    <td>V*</td>
    <td>V</td>
  </tr>
  <tr>
    <td>Protect critical data if a device is lost, stolen or confiscated</td>
    <td>BitLocker encryption</td>
    <td> BitLocker can leverage the TPM2.0 to encrypt and protect data”</td>
    <td>V</td>
    <td>V</td>
  </tr></tbody>
</table>

*Possible on some devices
