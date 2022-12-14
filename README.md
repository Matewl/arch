# Test log

## More info in Github.Actions: [![statusbadge](../../actions/workflows/buildtest.yml/badge.svg?branch=main&event=pull_request)](../../actions/workflows/buildtest.yml)
        
        
### Compile complited (build log, can be empty):
```
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:526:30: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rd = reg(rg).c_str();
                             ^~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:531:30: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rd = reg(rg).c_str();
                             ^~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:554:31: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rs1 = reg(rgs1).c_str();
                              ^~~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:555:30: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rd = reg(rgd).c_str();
                             ^~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:565:31: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rs1 = reg(rgs1).c_str();
                              ^~~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:566:31: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rs2 = reg(rgs2).c_str();
                              ^~~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:585:31: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rs1 = reg(rgs1).c_str();
                              ^~~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:586:31: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rs2 = reg(rgs2).c_str();
                              ^~~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:604:31: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rs1 = reg(rgs1).c_str();
                              ^~~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:605:30: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rd = reg(rgd).c_str();
                             ^~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:618:31: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rs1 = reg(rgs1).c_str();
                              ^~~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:619:30: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rd = reg(rgd).c_str();
                             ^~~~~~~~
/home/runner/work/spbsu-comp-arch22-lab3-Matewl/spbsu-comp-arch22-lab3-Matewl/main.cpp:620:31: warning: object backing the pointer will be destroyed at the end of the full-expression [-Wdangling-gsl]
            const char *rs2 = reg(rgs2).c_str();
                              ^~~~~~~~~
13 warnings generated.

```

### Output:
```
10074 <main>:
10074:	ff010113	   addi	sp, sp, -16
10078:	00112623	     sw	ra, 0(ra)
1007c:	030000ef	    jal	ra, 0x100ac <mmul>
10080:	00c12083	     lw	ra, 12(ra)
10084:	00000513	   addi	a0, a0, 0
10088:	01010113	   addi	sp, sp, 16
1008c:	00008067	   jalr	zero, 0(zero)
10090:	00000013	   addi	zero, zero, 0
10094:	00100137	    lui	sp,0x100
10098:	fddff0ef	    jal	ra, 0x10074 <main>
1009c:	00050593	   addi	a1, a1, 0
100a0:	00a00893	   addi	a7, a7, 10
100a4:	0ff0000f	unknown_instruction
100a8:	00000073	  ecall
100ac <mmul>:
100ac:	00011f37	    lui	t5,0x11
100b0:	124f0513	   addi	a0, a0, 292
100b4:	65450513	   addi	a0, a0, 1620
100b8:	124f0f13	   addi	t5, t5, 292
100bc:	e4018293	   addi	t0, t0, -448
100c0:	fd018f93	   addi	t6, t6, -48
100c4:	02800e93	   addi	t4, t4, 40
100c8 <L2>:
100c8:	fec50e13	   addi	t3, t3, -20
100cc:	000f0313	   addi	t1, t1, 0
100d0:	000f8893	   addi	a7, a7, 0
100d4:	00000813	   addi	a6, a6, 0
100d8 <L1>:
100d8:	00088693	   addi	a3, a3, 0
100dc:	000e0793	   addi	a5, a5, 0
100e0:	00000613	   addi	a2, a2, 0
100e4 <L0>:
100e4:	00078703	     lb	a4, 0(a4)
100e8:	00069583	     lh	a1, 0(a1)
100ec:	00178793	   addi	a5, a5, 1
100f0:	02868693	   addi	a3, a3, 40
100f4:	02b70733	    mul	a1, a1, a1
100f8:	00e60633	    add	a4, a4, a4
100fc:	fea794e3	    bne	a0, a0, 0x100e4 <L0>
10100:	00c32023	     sw	a2, 0(a2)
10104:	00280813	   addi	a6, a6, 2
10108:	00430313	   addi	t1, t1, 4
1010c:	00288893	   addi	a7, a7, 2
10110:	fdd814e3	    bne	t4, t4, 0x100d8 <L1>
10114:	050f0f13	   addi	t5, t5, 80
10118:	01478513	   addi	a0, a0, 20
1011c:	fa5f16e3	    bne	t0, t0, 0x100c8 <L2>
10120:	00008067	   jalr	zero, 0(zero)

Symbol Value              Size Type 	Bind     Vis       Index Name
[   0] 0x0                   0 NOTYPE   LOCAL    DEFAULT   UNDEF 
[   1] 0x10074               0 SECTION  LOCAL    DEFAULT       1 
[   2] 0x11124               0 SECTION  LOCAL    DEFAULT       2 
[   3] 0x0                   0 SECTION  LOCAL    DEFAULT       3 
[   4] 0x0                   0 SECTION  LOCAL    DEFAULT       4 
[   5] 0x0                   0 FILE     LOCAL    DEFAULT     ABS test.c
[   6] 0x11924               0 NOTYPE   GLOBAL   DEFAULT     ABS __global_pointer$
[   7] 0x118F4             800 OBJECT   GLOBAL   DEFAULT       2 b
[   8] 0x11124               0 NOTYPE   GLOBAL   DEFAULT       1 __SDATA_BEGIN__
[   9] 0x100AC             120 FUNC     GLOBAL   DEFAULT       1 mmul
[  10] 0x0                   0 NOTYPE   GLOBAL   DEFAULT   UNDEF _start
[  11] 0x11124            1600 OBJECT   GLOBAL   DEFAULT       2 c
[  12] 0x11C14               0 NOTYPE   GLOBAL   DEFAULT       2 __BSS_END__
[  13] 0x11124               0 NOTYPE   GLOBAL   DEFAULT       2 __bss_start
[  14] 0x10074              28 FUNC     GLOBAL   DEFAULT       1 main
[  15] 0x11124               0 NOTYPE   GLOBAL   DEFAULT       1 __DATA_BEGIN__
[  16] 0x11124               0 NOTYPE   GLOBAL   DEFAULT       1 _edata
[  17] 0x11C14               0 NOTYPE   GLOBAL   DEFAULT       2 _end
[  18] 0x11764             400 OBJECT   GLOBAL   DEFAULT       2 a

```

### Test output:
Readelf
```

Symbol table '.symtab' contains 19 entries:
   Num:    Value  Size Type    Bind   Vis      Ndx Name
     0: 00000000     0 NOTYPE  LOCAL  DEFAULT  UND 
     1: 00010074     0 SECTION LOCAL  DEFAULT    1 
     2: 00011124     0 SECTION LOCAL  DEFAULT    2 
     3: 00000000     0 SECTION LOCAL  DEFAULT    3 
     4: 00000000     0 SECTION LOCAL  DEFAULT    4 
     5: 00000000     0 FILE    LOCAL  DEFAULT  ABS test.c
     6: 00011924     0 NOTYPE  GLOBAL DEFAULT  ABS __global_pointer$
     7: 000118f4   800 OBJECT  GLOBAL DEFAULT    2 b
     8: 00011124     0 NOTYPE  GLOBAL DEFAULT    1 __SDATA_BEGIN__
     9: 000100ac   120 FUNC    GLOBAL DEFAULT    1 mmul
    10: 00000000     0 NOTYPE  GLOBAL DEFAULT  UND _start
    11: 00011124  1600 OBJECT  GLOBAL DEFAULT    2 c
    12: 00011c14     0 NOTYPE  GLOBAL DEFAULT    2 __BSS_END__
    13: 00011124     0 NOTYPE  GLOBAL DEFAULT    2 __bss_start
    14: 00010074    28 FUNC    GLOBAL DEFAULT    1 main
    15: 00011124     0 NOTYPE  GLOBAL DEFAULT    1 __DATA_BEGIN__
    16: 00011124     0 NOTYPE  GLOBAL DEFAULT    1 _edata
    17: 00011c14     0 NOTYPE  GLOBAL DEFAULT    2 _end
    18: 00011764   400 OBJECT  GLOBAL DEFAULT    2 a

```

Objdump
```

test.elf:     file format elf32-littleriscv

SYMBOL TABLE:
00010074 l    d  .text	00000000 .text
00011124 l    d  .bss	00000000 .bss
00000000 l    d  .comment	00000000 .comment
00000000 l    d  .riscv.attributes	00000000 .riscv.attributes
00000000 l    df *ABS*	00000000 test.c
00011924 g       *ABS*	00000000 __global_pointer$
000118f4 g     O .bss	00000320 b
00011124 g       .text	00000000 __SDATA_BEGIN__
000100ac g     F .text	00000078 mmul
00000000         *UND*	00000000 _start
00011124 g     O .bss	00000640 c
00011c14 g       .bss	00000000 __BSS_END__
00011124 g       .bss	00000000 __bss_start
00010074 g     F .text	0000001c main
00011124 g       .text	00000000 __DATA_BEGIN__
00011124 g       .text	00000000 _edata
00011c14 g       .bss	00000000 _end
00011764 g     O .bss	00000190 a



Disassembly of section .text:

00010074 <main>:
   10074:	ff010113          	addi	sp,sp,-16
   10078:	00112623          	sw	ra,12(sp)
   1007c:	030000ef          	jal	ra,100ac <mmul>
   10080:	00c12083          	lw	ra,12(sp)
   10084:	00000513          	addi	a0,zero,0
   10088:	01010113          	addi	sp,sp,16
   1008c:	00008067          	jalr	zero,0(ra)
   10090:	00000013          	addi	zero,zero,0
   10094:	00100137          	lui	sp,0x100
   10098:	fddff0ef          	jal	ra,10074 <main>
   1009c:	00050593          	addi	a1,a0,0
   100a0:	00a00893          	addi	a7,zero,10
   100a4:	0ff0000f          	fence	iorw,iorw
   100a8:	00000073          	ecall

000100ac <mmul>:
   100ac:	00011f37          	lui	t5,0x11
   100b0:	124f0513          	addi	a0,t5,292 # 11124 <__DATA_BEGIN__>
   100b4:	65450513          	addi	a0,a0,1620
   100b8:	124f0f13          	addi	t5,t5,292
   100bc:	e4018293          	addi	t0,gp,-448 # 11764 <a>
   100c0:	fd018f93          	addi	t6,gp,-48 # 118f4 <b>
   100c4:	02800e93          	addi	t4,zero,40
   100c8:	fec50e13          	addi	t3,a0,-20
   100cc:	000f0313          	addi	t1,t5,0
   100d0:	000f8893          	addi	a7,t6,0
   100d4:	00000813          	addi	a6,zero,0
   100d8:	00088693          	addi	a3,a7,0
   100dc:	000e0793          	addi	a5,t3,0
   100e0:	00000613          	addi	a2,zero,0
   100e4:	00078703          	lb	a4,0(a5)
   100e8:	00069583          	lh	a1,0(a3)
   100ec:	00178793          	addi	a5,a5,1
   100f0:	02868693          	addi	a3,a3,40
   100f4:	02b70733          	mul	a4,a4,a1
   100f8:	00e60633          	add	a2,a2,a4
   100fc:	fea794e3          	bne	a5,a0,100e4 <mmul+0x38>
   10100:	00c32023          	sw	a2,0(t1)
   10104:	00280813          	addi	a6,a6,2
   10108:	00430313          	addi	t1,t1,4
   1010c:	00288893          	addi	a7,a7,2
   10110:	fdd814e3          	bne	a6,t4,100d8 <mmul+0x2c>
   10114:	050f0f13          	addi	t5,t5,80
   10118:	01478513          	addi	a0,a5,20
   1011c:	fa5f16e3          	bne	t5,t0,100c8 <mmul+0x1c>
   10120:	00008067          	jalr	zero,0(ra)

```