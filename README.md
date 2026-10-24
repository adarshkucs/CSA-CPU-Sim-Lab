# CSA-CPU-Sim-Lab# Computer System Architecture – CPU Sim Lab

| | |
|---|---|
| **Name** | < SubhamSingh> |
| **Roll No.** | <265700626> |
| **Course / Semester** | <Bsc(hons)computer science,semester-1> |
| **College** | Ramanujan College, University of Delhi |
| **Paper** | Computer System Architecture |

Simulation of Mano's Basic Computer using **CPU Sim 4.0.11** (Java 8 with JavaFX).
Each practical has its own folder containing the program (where applicable) and the screenshots of its output.

## Index of Practicals

| No. | Practical | Folder |
|---|---|---|
| 1 | Create a machine based on the Basic Computer architecture | [Practical_01_Create_Machine](CSA-CPU-Sim-Lab/Practical_01_Create_Machine) |
| 2 | Create the Fetch routine of the instruction cycle | [Practical_02_Fetch_Routine](CSA-CPU-Sim-Lab/Practical_02_Fetch_Routine) |
| 3 | ADD operation on two user-entered numbers | [Practical_03_ADD](CSA-CPU-Sim-Lab/Practical_03_ADD) |
| 4 | SUBTRACT operation on two user-entered numbers | [Practical_04_SUBTRACT](CSA-CPU-Sim-Lab/Practical_04_SUBTRACT) |
| 5 | Logical operations AND, OR, NOT, XOR, NOR, NAND | [Practical_05_Logical_Ops](CSA-CPU-Sim-Lab/Practical_05_Logical_Ops) |
| 6 | Memory-reference instructions ADD, LDA, STA, BUN, ISZ | [Practical_06_Memory_Reference](CSA-CPU-Sim-Lab/Practical_06_Memory_Reference) |
| 7 | Register-reference instructions CLA, CMA, CME, HLT | [Practical_07_CLA_CMA_CME_HLT](CSA-CPU-Sim-Lab/Practical_07_CLA_CMA_CME_HLT) |
| 8 | Register-reference instructions INC, SPA, SNA, SZE | [Practical_08_INC_SPA_SNA_SZE](CSA-CPU-Sim-Lab/Practical_08_INC_SPA_SNA_SZE) |
| 9 | Register-reference instructions CIR, CIL | [Practical_09_CIR_CIL](CSA-CPU-Sim-Lab/Practical_09_CIR_CIL) |
| 10 | Sum of integers until a negative number is read | [Practical_10_Sum_Until_Negative](CSA-CPU-Sim-Lab/Practical_10_Sum_Until_Negative) |
| 11 | Sum of integers until zero is read | [Practical_11_Sum_Until_Zero](CSA-CPU-Sim-Lab/Practical_11_Sum_Until_Zero) |

## Repository structure

```
CSA-CPU-Sim-Lab/
├── README.md
├── Practical_01_Create_Machine/
│   ├── BasicComputer.cpu        <- the machine used by all other practicals
│   └── screenshots/
├── Practical_02_Fetch_Routine/
│   └── screenshots/
├── Practical_03_ADD/
│   ├── P03_ADD.a
│   └── screenshots/
│   ...
└── Practical_11_Sum_Until_Zero/
    ├── P11_SUM_UNTIL_ZERO.a
    └── screenshots/
```

## How to run

1. Install **Java 8 with JavaFX** (for example Azul Zulu JDK FX 8) and download **CPU Sim 4.0.11**.
2. Start CPU Sim (`Cpusim4.bat`).
3. **File → Open machine…** and choose `Practical_01_Create_Machine/BasicComputer.cpu`.
4. **File → Open text…** and choose the `.a` program from the practical's folder.
5. Press **Ctrl+2** (assemble and load), then:
   - **Ctrl+R** to run, or
   - **Ctrl+D** to enter debug mode and use **Step by Instr** / **Step by Micro**.
6. For programs that read input, type a number in the yellow console and press **Enter**.
7. **Example (Practical 3):** open `Practical_03_ADD/P03_ADD.a`, press Ctrl+2, then Ctrl+R, and enter `25` and `17`. The console shows `Output: 42`.

## Notes
- Practical 2 uses the same machine file as Practical 1; its screenshots show the fetch routine executed one microinstruction at a time .
- Register values in the debug traces are shown in **Unsigned Dec**; the RAM pane is shown in **Hex**.
