RUGE
====

Realization of uCore on Goldfish Emulator

## Goldfish 上的 uCore 操作系统实现

本课程共 18 周，可分为 3 个阶段，1基础(6周)，2提高(9周)，3选修(3周)

stage 1: week 1 ~ 6
基础阶段，通过6周时间快速构建一个OS的雏形，能够实现 Shell 功能，运行用户程序。
	
	lab1.1: Bootloader + ELF OS + UART driver
	  掌握3个核心概念：loader加载器, elf可执行文件格式, driver设备驱动
	
	lab1.2: Interrupt + Mode + Context Switch
		掌握3个核心概念：int中断, mode处理器工作模式, context处理器上下文
		
	lab1.3: Physical Memory Management
		掌握3个核心概念：heap堆, alloc/free分配和回收, slab分配机制
	
	lab1.4: Process/PCB + Timer + Scheduling
		掌握3个核心概念：process/pcb进程控制块, timer时间片, scheduling调度策略
	
	lab1.5: IPC + Mutex + Semaphore
		掌握3个核心概念：ipc进程间通讯, mutex互斥锁，sem信号量
	
	lab1.6: Filesystem/namei + OSloader + Shell
		掌握3个核心概念：fs/namei文件名索引数据块, os加载器，shell外壳/用户界面

	
stage 2: week 7 ~ 15
提高阶段，通过9周时间扩展对操作系统各个方面的深化认识，能够实现 WebServer 功能，基于硬件平台实践实现。

	lab2.1: Virtual memory management 
		虚拟内存管理, 包括 MMU，页表，ioremap，内核空间和用户空间等概念
	
	lab2.2: page fault handler & system call
		page fault 缺页异常，swap in/out 换入换出，系统调用概念（异常处理）
	
	lab2.3: memory map 
		内存映射，进程空间，share memory 共享内存
	
	lab2.4: scheduling method
		RoundRobin(RR) 轮转调度策略/ preemptive 抢占式内核 
	
	lab2.5: IPC
		进程间通讯详解，包括pipe管道，event事件，mailbox邮箱，signal信号
		
	lab2.6: VFS 
		虚拟文件系统，simple fs，exec系统调用
	
	lab2.7: net driver
		网卡驱动，了解phy/mac层（支持DM9000/CS8900网卡）
	
	lab2.8: Socket
		网络协议，了解ip/tcp/udp层（lwip协议栈，socket编程接口）
	
	lab2.9: WebServer
		综合项目：完成一个OS+web服务器，巩固以上概念（必做内容）

stage 3: week 16 ~ 18
选修内容 （大作业）

	lab3.1: 为内核实现一种新的调度策略，MultiLevel Feedback Queue(MLFQ) scheduling methodmethod
	属于进程管理方向：
	
	lab3.2: 为虚存管理引入交换文件，swap in/out including page replacement 
	属于存储管理方向：
	
	lab3.3: 文件管理：为用户进程运行引入动态链接，dynamic-linker, shared library
	属于文件系统方向：
