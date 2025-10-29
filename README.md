# RansomwareShield - Augmented Dataset

This repository contains the **augmented dataset** used for evaluating the **RansomwareShield** model. The dataset was created to analyze ransomware behavior through various static and dynamic features collected from a variety of **Android** and **Windows** executables.

## Dataset Overview

- **Total Samples**: 62,485 (with an equal distribution of benign and malicious samples)
- **Number of Features**: 41 features
  - **Static Features**: Permissions, API usage, security flags, etc.
  - **Dynamic Features**: Runtime behavior, network activity, system calls.
  - **Target Label**: `Benign` (0) or `Malicious` (1)

## Features

The dataset contains the following key columns:

| Column Name                | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| **FileName**                | The name of the executable file.                                             |
| **md5Hash**                 | The MD5 hash of the file for integrity verification.                         |
| **Machine**                 | Architecture of the machine (32-bit/64-bit).                                |
| **DebugSize**               | Size of the debug section in the file.                                      |
| **DebugRVA**                | The Relative Virtual Address (RVA) of the debug section.                    |
| **MajorImageVersion**       | Major version of the image (executable).                                    |
| **MajorOSVersion**          | Major version of the operating system.                                      |
| **ExportRVA**               | The RVA for exported functions.                                             |
| **ExportSize**              | Size of the export section.                                                 |
| **IatVRA**                  | RVA of the Import Address Table (IAT).                                      |
| **MajorLinkerVersion**      | Major version of the linker.                                                |
| **MinorLinkerVersion**      | Minor version of the linker.                                                |
| **NumberOfSections**        | Number of sections in the executable.                                       |
| **SizeOfStackReserve**      | Size of the stack reserve for the executable.                               |
| **DllCharacteristics**      | Characteristics of the DLL.                                                 |
| **ResourceSize**            | Size of resources in the executable.                                        |
| **BitcoinAddresses**        | Any Bitcoin addresses found in the file.                                    |
| **Benign**                  | Label indicating whether the file is benign (0) or malicious (1).          |
| **dyn_syscall_rate**        | Rate of system calls made by the executable during runtime.                 |
| **dyn_reg_key_mod_count**   | Count of registry key modifications.                                        |
| **dyn_file_entropy**        | Entropy (complexity) of the file during execution.                          |
| **dyn_mem_usage_mb**        | Memory usage during runtime (in MB).                                        |
| **dyn_api_seq_score**       | Score based on the sequence of API calls.                                   |
| **dyn_net_conn_attempts**   | Number of network connection attempts made during execution.               |
| **ASLR**                    | Address Space Layout Randomization (enabled or disabled).                   |
| **DEP**                     | Data Execution Prevention status.                                           |
| **import_count**            | The number of imported functions in the executable.                         |
| **is_packed**               | Indicates whether the executable is packed (1) or not (0).                  |
| **enc_keyword_score**       | Score based on the presence of encrypted keywords in the executable.        |
| **perm_CAMERA**             | Permission to access the camera (1 = granted, 0 = not granted).             |
| **perm_SMS**                | Permission to send SMS (1 = granted, 0 = not granted).                      |
| **perm_STORAGE**            | Permission to access storage (1 = granted, 0 = not granted).               |
| **api_SEND_SMS**            | Whether the `SEND_SMS` API is used by the executable (1 = used).            |
| **url_count**               | The number of URLs accessed by the executable.                              |
| **ip_count**                | The number of IP addresses accessed by the executable.                      |
| **manifest_debuggable**     | Whether the app’s manifest is marked as debuggable (1 = true, 0 = false).   |
| **ent_camera**              | Indicator if camera functionality is used (1 = used, 0 = not used).         |
| **ent_keychain**            | Whether keychain functionality is used (1 = used, 0 = not used).           |
| **api_crypto_lib**          | Whether the executable uses cryptographic libraries (1 = used).             |
| **uses_swift**              | Whether the executable uses Swift programming language (1 = used).          |
| **suspicious_domain_calls** | Count of suspicious domain calls made by the executable during execution.   |

## License

This dataset is available under the **MIT License** for research and educational purposes. Please cite the repository if you use this dataset in your work.

## Contact
email : duttosourav8@gmail.com
For any questions, issues, or collaborations, please feel free to reach out.

