# ACPI说明
|    名称    |     硬件      |   说明   |   是否需要   |
| :--------: | :-----------: | :------ | :------ |
| SSDT-AWAC    | H170              | Coffee Lake处理器搭配的主板才有AWAC功能并需要启用，我们的主板是H170魔改使用的8100，并不需要。旨在修复时钟问题 | 不需要 |
| SSDT-DEGPU   | GTX 1050Ti Laptop | 不禁用的话睡眠受到影响无法正常唤醒并启用iGPU点亮屏幕 | 需要 |
| SSDT-EC      | H170              | 已屏蔽  | 需要 |
| SSDT-USBX    | H170              | 已驱动  | 需要 |
| SSDT-EC-USBX | H170              | EC和USBX的合并版本 | 需要 |
| SSDT-PLUG    | H170              | 和CPU电源管理有关 | 需要 |
| SSDT-PMC     | H170              | Coffee Lake处理器搭配的主板才需要启用，我们的主板是H170魔改使用的8100。旨在带来“back NVRAM”功能 | 不需要 |
| SSDT-PNLF    | H170              | 修复背光问题，如果出现屏幕闪烁问题，可能和这个文件或者仿冒cpuid有关 | 需要 |

- 我的配置默认使用的prebuild版本
- 后缀带“SPEC”的文件版本是使用SSDTTime工具自动生成的优化版本。该版本占用空间更小，对提升开机速度有一定提升（但不大，0.5s）
- dsl通过编译得到aml文件，aml文件反编译可以得到dsl，并看到源码
- 根据OpenCore-Install-Guide说明，不需要的ACPI文件最好被删除，不管有没有被引用。该目录只需要留下被启用的aml文件
