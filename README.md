# GlossHook
A simple Android arm Hook library.

## English
Features:
- Support Android 5.0 - 14.0

- Support for Android Thumb/ARM/ARM64 architectures.

- Implementation of Inline Hook and Got/Plt Hook

- Support for hooking a single branch instruction (BL, BLX) calling a function. Sometimes you may only need to hook one specific call site of a function, rather than all call sites.

- Support for hooking short functions (minimum 4 bytes).

- Support for hook patching at any address within executable code. You can read and write registers, stack, and call other functions within your hooked function.

- After hooking, you can choose to either callback the original function or directly replace the function.

- Support for multiple hooks at the same location.

- For multiple hooks at the same location, you can enable/disable/remove any individual hook or all hooks using the hook pointer or hook address. Enabling/disabling/removing one hook does not affect other hooks at the same location.

- If multiple users use GlossHook to hook the same location, any user can enable/disable/remove other hooks using the hook pointer.

- Provides a function to get the number of hooks at a specific location.

- Support for replacing a user function that is already being hooked.

- Provides common API functions for library lookup, library information, symbol address retrieval, memory read/write, and memory permission removal, etc.

## 中文说明
一个安卓ArmHook库，它适用于游戏Mod的制作。

### 特性
* 支持安卓5.0 ~ 14.0

* 支持Thumb/Arm/Arm64的InlineHook和PltHook、GotHook

* 支持Hook分支指令(BL BLX)，有时候你可能只需要hook函数其中一处调用点，而不是函数的全部调用点

* 能对linker中dl系列函数进行hook

* 支持短函数Hook，最短4字节的函数

* 能Hook可执行代码任意位置，访问该位置的寄存器，插入函数调用

* Hook一个函数后，可调用原函数，也可不调用直接替换函数

* 支持对同一个位置的多次hook

* 提供常用的库查找、获取符号地址、读写内存、解除内存权限等API

* 其它待更新ing
