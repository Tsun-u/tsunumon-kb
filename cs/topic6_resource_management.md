# Topic 6: Resource Management

> HL only

## Key Concepts

### 6.1 System Resources

#### Identification of Resources
- **System resources**: CPU time, memory, storage, network bandwidth, peripherals
- Resource management: allocation, scheduling, and deallocation
- The operating system acts as the central manager for all system resources

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
- **Deadlock**: a situation where two or more processes are permanently blocked because each holds a resource the other needs and neither will give it up
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
| **Virtual memory** | A technique that makes disk space appear as extra RAM, allowing programs larger than physical memory to run |
| **Paging** | Splitting memory into equal-sized pages and mapping virtual page addresses to physical frames |
| **Thrashing** | A performance collapse where the system spends nearly all its time swapping pages in and out of disk rather than doing useful work |
| **Process** | A running instance of a program, complete with its own memory space and state |
| **Scheduling** | The OS mechanism that decides which process uses the CPU next and for how long |
| **Deadlock** | A standstill where a set of processes are each waiting indefinitely for a resource held by another in the group |
| **Round Robin** | A scheduling approach that cycles through all ready processes, giving each the same fixed time slice before moving to the next |
| **Cache** | A small, extremely fast memory bank that stores recently or frequently accessed data to reduce average access time |

## Common Misconceptions

1. **"More RAM eliminates the need for virtual memory"** — Virtual memory also provides memory isolation and protection between processes, so it serves purposes beyond simply extending capacity.
2. **"Multitasking means multiple processes run simultaneously on a single core"** — On one core, the CPU switches between processes so rapidly it appears simultaneous; genuine parallelism requires multiple cores.
3. **"Deadlock is the same as a crash"** — In a deadlock the operating system is still running normally; only the blocked processes are stuck.
4. **"The fastest scheduling algorithm is always best"** — Scheduling involves trade-offs between throughput, response time, fairness, and resource utilization.

## Comparison with AP CS

- AP CS A does not cover operating systems or resource management
- AP CS Principles briefly mentions the role of operating systems
- IB HL's coverage of memory management, scheduling, and deadlock is unique among high-school CS curricula
- This content is closer to university-level operating systems courses
