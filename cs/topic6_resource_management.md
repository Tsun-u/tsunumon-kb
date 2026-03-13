# Topic 6: Resource Management

> HL only

## Key Concepts

### 6.1 System Resources

#### Identification of Resources
- **System resources**: CPU time, memory, storage, network bandwidth, peripherals
- Resource management: allocation, scheduling, and deallocation
- Role of the operating system in resource management

#### Resource Limitations
- Limited CPU time → need for scheduling
- Limited memory → need for memory management
- Limited storage → need for file management
- Resource contention: multiple processes competing for the same resource

### 6.2 Role of the Operating System

#### Memory Management
- **Primary memory** allocation and deallocation
- **Paging**: memory divided into fixed-size pages; virtual addresses mapped to physical
- **Segmentation**: memory divided into variable-size segments based on logical divisions
- **Virtual memory**: using disk space as extension of RAM
  - **Page swapping**: moving pages between RAM and disk
  - **Thrashing**: excessive page swapping that degrades performance
- **Cache memory**: small, fast memory between CPU and RAM
  - Cache hit vs. cache miss

#### Process Management
- **Process**: a program in execution
- Process states: new → ready → running → waiting → terminated
- **Scheduling algorithms**:
  - **First Come, First Served (FCFS)**: simple, no preemption; can cause convoy effect
  - **Shortest Job First (SJF)**: minimizes average waiting time; requires knowing job length
  - **Round Robin (RR)**: each process gets a time quantum; fair but context switching overhead
  - **Priority scheduling**: processes assigned priorities; risk of starvation
- **Preemptive vs. non-preemptive scheduling**
- **Multitasking**: CPU rapidly switches between processes (time-sharing)
- **Deadlock**: two or more processes each waiting for resources held by the other
  - Conditions: mutual exclusion, hold and wait, no preemption, circular wait

### 6.3 File Management

- File systems: FAT, NTFS, ext4, HFS+
- Directory structures: hierarchical (tree), flat
- File operations: create, read, write, delete, rename, move
- **Access rights**: read, write, execute; user, group, other
- File compression: lossy vs. lossless

### 6.4 Security Considerations

- User authentication and authorization
- Access control lists (ACLs)
- Malware protection
- Encryption of stored data

## Key Terminology

| Term | Definition |
|------|-----------|
| **Virtual memory** | Technique using disk space to extend available RAM |
| **Paging** | Dividing memory into fixed-size blocks (pages) for management |
| **Thrashing** | Excessive page swapping that severely degrades system performance |
| **Process** | An instance of a program currently being executed |
| **Scheduling** | Determining which process gets CPU time and for how long |
| **Deadlock** | Situation where processes are permanently blocked, each waiting for resources held by others |
| **Round Robin** | Scheduling algorithm giving each process equal time slices |
| **Cache** | Small, fast memory providing quick access to frequently used data |

## Common Misconceptions

1. **"More RAM eliminates the need for virtual memory"** -- Even with ample RAM, virtual memory provides memory protection and allows running programs larger than physical memory.
2. **"Multitasking means multiple processes run simultaneously on a single core"** -- On a single core, the CPU rapidly switches between processes; true parallelism requires multiple cores.
3. **"Deadlock is the same as a crash"** -- Deadlock means processes are stuck waiting; the system is still running but those processes are blocked.
4. **"The fastest scheduling algorithm is always best"** -- Scheduling involves trade-offs between throughput, response time, fairness, and resource utilization.

## Comparison with AP CS

- AP CS A does not cover operating systems or resource management
- AP CS Principles briefly mentions the role of operating systems
- IB HL's coverage of memory management, scheduling, and deadlock is unique among high-school CS curricula
- This content is closer to university-level operating systems courses
