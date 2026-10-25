# Microsoft Visual C++ Runtime Provenance

The listed DLLs are present in the current 0.66b baseline payload. SHA-256 values below were compared against the installed Visual Studio 18 Community VC redist/toolchain files during the license hardening task.

| Payload path | File version | Payload SHA-256 | Exact local Visual Studio file hash match | Status |
|---|---:|---|---|---|
| `Modules/Upscalers/RealCUGAN/20220728/bin/c/vcomp140.dll` | 14.32.31332.0 | `54FE6B087528B33C2969143D811EB62F1BD49071D37DE9DB0745FC079764D698` | No match in scanned Visual Studio 18 Community VC tree | Provenance unresolved |
| `Modules/Upscalers/RealESRGAN/v0.2.0/bin/e/vcomp140.dll` | 14.31.31103.0 | `8F72EF2E483465444B2059FC6744D6CB22CD8D8A27F6FA56BEFD2A42DCD0F78B` | No match in scanned Visual Studio 18 Community VC tree | Provenance unresolved |
| `Modules/Upscalers/DAT2/runtime/msvcp140.dll` | 14.51.36247.0 | `7C26614E1D733892C2DEAC7E245CE115504B1D80592DD0A01B08E3E5A55F89CA` | Byte-identical hash match under installed Visual Studio VC redist | Source copy established; release eligibility still governed by Microsoft's terms |
| `Modules/Upscalers/DAT2/runtime/vcruntime140.dll` | 14.51.36247.0 | `D1F4225DF2CD877DBF130D5668A021DCE3F94118455FF5EC952061C30AFC9CE7` | Byte-identical hash match under installed Visual Studio VC redist | Source copy established; release eligibility still governed by Microsoft's terms |
| `Modules/Upscalers/DAT2/runtime/vcruntime140_1.dll` | 14.51.36247.0 | `A7146C08F89FE5B04541AB507CDB59FF7B44534D4BA3C668A426C6450A03434E` | Byte-identical hash match under installed Visual Studio VC redist | Source copy established; release eligibility still governed by Microsoft's terms |

All five DLLs had a valid Microsoft Authenticode signature when inspected. A valid signature establishes signer identity/integrity; it does not independently establish how the particular payload copy was obtained or whether redistribution terms are satisfied.

Microsoft's official redistribution guidance: https://learn.microsoft.com/en-us/cpp/windows/redistributing-visual-cpp-files?view=msvc-170

No runtime binaries were modified or replaced in this task.
