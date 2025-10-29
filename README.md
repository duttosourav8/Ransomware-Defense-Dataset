Column Descriptions for dataset_augmented_crossplatform.csv:

FileName: The name of the file (executable).

md5Hash: The MD5 hash of the file (used for file integrity checks).

Machine: Machine architecture (e.g., 32-bit, 64-bit).

DebugSize: Size of the debug section in the file.

DebugRVA: The Relative Virtual Address (RVA) for the debug section.

MajorImageVersion: The major version of the image (binary executable).

MajorOSVersion: The major version of the operating system.

ExportRVA: The RVA for exported functions.

ExportSize: Size of the exported functions section.

IatVRA: The RVA of the Import Address Table (IAT).

MajorLinkerVersion: Major version of the linker.

MinorLinkerVersion: Minor version of the linker.

NumberOfSections: The number of sections in the executable.

SizeOfStackReserve: Size of the stack reserve for the executable.

DllCharacteristics: Characteristics of the DLL (Dynamic Link Library).

ResourceSize: Size of resources in the executable.

BitcoinAddresses: Any Bitcoin addresses found in the executable.

Benign: Label indicating whether the file is benign (0) or malicious (1).

dyn_syscall_rate: The rate of system calls made by the executable during runtime.

dyn_reg_key_mod_count: The count of modified registry keys during execution.

dyn_file_entropy: The entropy (complexity) of the file during execution.

dyn_mem_usage_mb: Memory usage (in MB) during runtime.

dyn_api_seq_score: A score related to the sequence of API calls made by the executable.

dyn_net_conn_attempts: Number of network connection attempts made by the executable.

ASLR: Address Space Layout Randomization (binary is protected by ASLR).

DEP: Data Execution Prevention status.

import_count: The number of imported functions used by the executable.

is_packed: Indicates if the executable is packed or obfuscated.

enc_keyword_score: Score based on the presence of encrypted keywords.

perm_CAMERA: Permission to access the camera (1 = granted, 0 = not granted).

perm_SMS: Permission to send SMS (1 = granted, 0 = not granted).

perm_STORAGE: Permission to access storage (1 = granted, 0 = not granted).

api_SEND_SMS: Whether the SEND_SMS API is used by the executable (1 = used, 0 = not used).

url_count: The number of URLs accessed by the executable.

ip_count: The number of IP addresses accessed by the executable.

manifest_debuggable: Whether the app’s manifest file is marked as debuggable (1 = true, 0 = false).

ent_camera: Indicator if camera-related functionality is used in the executable (1 = used, 0 = not used).

ent_keychain: Indicator if keychain-related functionality is used (e.g., access to stored credentials) (1 = used, 0 = not used).

api_crypto_lib: Whether the executable uses cryptographic libraries (1 = used, 0 = not used).

uses_swift: Whether the executable uses Swift programming language features (1 = used, 0 = not used).

suspicious_domain_calls: The count of suspicious domain calls made during execution.
