# ARMv7 Prebuilt Tools

Prebuilt small tools for ARMv7 (not ARMv7hf) devices, e.g. older ASUS routers.

This repository contains **precompiled binaries** of selected open-source tools
for ARMv7 devices that are often not provided upstream, or are only released for
ARMv7 hard-float (`armv7hf`) targets.  
Some binaries are compiled from source; others are taken from official releases
and stripped for smaller size.

> **Note:** All tools are licensed under their respective upstream licenses.
> This repository only redistributes compiled binaries for convenience.  
> Please check each project's LICENSE file for details.

---

## Tools Included

| Tool | Source | License | Notes |
|------|--------|---------|-------|
| **dnsmasq** | [simonchen/dnsmasq](https://github.com/simonchen/dnsmasq) | GPL-3.0 | Upstream only provides `armv7hf`; built for `armv7` |
| **dufs** | [sigoden/dufs](https://github.com/sigoden/dufs) | MIT or Apache-2.0 | Upstream only provides `armv7hf`; built for `armv7` |
| **iperf** | [esnet/iperf](https://github.com/esnet/iperf) | BSD-3-Clause | No official ARM release; built for `armv7` |
| **tinyproxy** | [tinyproxy/tinyproxy](https://github.com/tinyproxy/tinyproxy) | GPL-2.0 | Source only; built for `armv7` |
| **wol** | [nashaofu/wol](https://github.com/nashaofu/wol) | Apache-2.0 | Official ARMv7 binary available; here it is stripped to reduce size |

---

## Build / Modification Notes

- **Architecture:** ARMv7 (soft-float ABI, `armv7`), unless otherwise stated.
- **Toolchain:** Prebuilt using cross-compilation toolchains (musl / static linking where possible).
- **Stripped:** Some binaries have been stripped (`strip`) to reduce file size.
- **Static Builds:** Certain tools are statically linked for portability.

---

## Related Projects

- [therealsaumil/static-arm-bins](https://github.com/therealsaumil/static-arm-bins) — A large collection of statically compiled ARM tools.

---

## License

This repository **does not** impose an additional license.  
Each binary is distributed under the license of its upstream project.

The original LICENSE files from each project are included in the `licenses/` directory or linked above.  
Please refer to them for the applicable terms and conditions.
