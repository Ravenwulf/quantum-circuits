# Quantum Circuits


## NOT Gate
NOT with input 0 gives output 1
```
           ░ ┌───┐ ░ ┌─┐
  q: ─|0>──░─┤ X ├─░─┤M├
           ░ └───┘ ░ └╥┘
c: 1/═════════════════╩═
                      0 
```

NOT with input 1 gives output 0
```
          ┌───┐ ░ ┌───┐ ░ ┌─┐
  q: ─|0>─┤ X ├─░─┤ X ├─░─┤M├
          └───┘ ░ └───┘ ░ └╥┘
c: 1/══════════════════════╩═
                           0 
```

## XOR Gate
XOR with inputs 0 0 gives output 0
```
           ░            ░    
q_0: ─|0>──░───■────────░────
           ░   │        ░    
q_1: ─|0>──░───┼────■───░────
           ░ ┌─┴─┐┌─┴─┐ ░ ┌─┐
q_2: ──────░─┤ X ├┤ X ├─░─┤M├
           ░ └───┘└───┘ ░ └╥┘
c: 1/══════════════════════╩═
                           0 
```
XOR with inputs 0 1 gives output 1
```
                ░            ░    
q_0: ─|0>───────░───■────────░────
          ┌───┐ ░   │        ░    
q_1: ─|0>─┤ X ├─░───┼────■───░────
          └───┘ ░ ┌─┴─┐┌─┴─┐ ░ ┌─┐
q_2: ───────────░─┤ X ├┤ X ├─░─┤M├
                ░ └───┘└───┘ ░ └╥┘
c: 1/═══════════════════════════╩═
                                0 
```
XOR with inputs 1 0 gives output 1
```
          ┌───┐ ░            ░    
q_0: ─|0>─┤ X ├─░───■────────░────
          └───┘ ░   │        ░    
q_1: ─|0>───────░───┼────■───░────
                ░ ┌─┴─┐┌─┴─┐ ░ ┌─┐
q_2: ───────────░─┤ X ├┤ X ├─░─┤M├
                ░ └───┘└───┘ ░ └╥┘
c: 1/═══════════════════════════╩═
                                0 
```
XOR with inputs 1 1 gives output 0
```
          ┌───┐ ░            ░    
q_0: ─|0>─┤ X ├─░───■────────░────
          ├───┤ ░   │        ░    
q_1: ─|0>─┤ X ├─░───┼────■───░────
          └───┘ ░ ┌─┴─┐┌─┴─┐ ░ ┌─┐
q_2: ───────────░─┤ X ├┤ X ├─░─┤M├
                ░ └───┘└───┘ ░ └╥┘
c: 1/═══════════════════════════╩═
                                0 
```

## AND Gate
AND with inputs 0 0 gives output 0
```
           ░       ░    
q_0: ─|0>──░───■───░────
           ░   │   ░    
q_1: ─|0>──░───■───░────
           ░ ┌─┴─┐ ░ ┌─┐
q_2: ──────░─┤ X ├─░─┤M├
           ░ └───┘ ░ └╥┘
c: 1/═════════════════╩═
                      0 
```
AND with inputs 0 1 gives output 0
```
                ░       ░    
q_0: ─|0>───────░───■───░────
          ┌───┐ ░   │   ░    
q_1: ─|0>─┤ X ├─░───■───░────
          └───┘ ░ ┌─┴─┐ ░ ┌─┐
q_2: ───────────░─┤ X ├─░─┤M├
                ░ └───┘ ░ └╥┘
c: 1/══════════════════════╩═
                           0 
```
AND with inputs 1 0 gives output 0
```
          ┌───┐ ░       ░    
q_0: ─|0>─┤ X ├─░───■───░────
          └───┘ ░   │   ░    
q_1: ─|0>───────░───■───░────
                ░ ┌─┴─┐ ░ ┌─┐
q_2: ───────────░─┤ X ├─░─┤M├
                ░ └───┘ ░ └╥┘
c: 1/══════════════════════╩═
                           0 
```
AND with inputs 1 1 gives output 1
```
          ┌───┐ ░       ░    
q_0: ─|0>─┤ X ├─░───■───░────
          ├───┤ ░   │   ░    
q_1: ─|0>─┤ X ├─░───■───░────
          └───┘ ░ ┌─┴─┐ ░ ┌─┐
q_2: ───────────░─┤ X ├─░─┤M├
                ░ └───┘ ░ └╥┘
c: 1/══════════════════════╩═
                           0 
```

## NAND Gate
NAND with inputs 0 0 gives output 1
```
           ░            ░    
q_0: ─|0>──░───■────────░────
           ░   │        ░    
q_1: ─|0>──░───■────────░────
           ░ ┌─┴─┐┌───┐ ░ ┌─┐
q_2: ──────░─┤ X ├┤ X ├─░─┤M├
           ░ └───┘└───┘ ░ └╥┘
c: 1/══════════════════════╩═
                           0 
```
NAND with inputs 0 1 gives output 1
```
                ░            ░    
q_0: ─|0>───────░───■────────░────
          ┌───┐ ░   │        ░    
q_1: ─|0>─┤ X ├─░───■────────░────
          └───┘ ░ ┌─┴─┐┌───┐ ░ ┌─┐
q_2: ───────────░─┤ X ├┤ X ├─░─┤M├
                ░ └───┘└───┘ ░ └╥┘
c: 1/═══════════════════════════╩═
                                0 
```
NAND with inputs 1 0 gives output 1
```
          ┌───┐ ░            ░    
q_0: ─|0>─┤ X ├─░───■────────░────
          └───┘ ░   │        ░    
q_1: ─|0>───────░───■────────░────
                ░ ┌─┴─┐┌───┐ ░ ┌─┐
q_2: ───────────░─┤ X ├┤ X ├─░─┤M├
                ░ └───┘└───┘ ░ └╥┘
c: 1/═══════════════════════════╩═
                                0 
```
NAND with inputs 1 1 gives output 0
```
          ┌───┐ ░            ░    
q_0: ─|0>─┤ X ├─░───■────────░────
          ├───┤ ░   │        ░    
q_1: ─|0>─┤ X ├─░───■────────░────
          └───┘ ░ ┌─┴─┐┌───┐ ░ ┌─┐
q_2: ───────────░─┤ X ├┤ X ├─░─┤M├
                ░ └───┘└───┘ ░ └╥┘
c: 1/═══════════════════════════╩═
                                0 
```

## OR Gate
OR with inputs 0 0 gives output 0
```
           ░                 ░    
q_0: ─|0>──░───■─────────■───░────
           ░   │         │   ░    
q_1: ─|0>──░───┼────■────■───░────
           ░ ┌─┴─┐┌─┴─┐┌─┴─┐ ░ ┌─┐
q_2: ─|0>──░─┤ X ├┤ X ├┤ X ├─░─┤M├
           ░ └───┘└───┘└───┘ ░ └╥┘
c: 1/═══════════════════════════╩═
                                0 
```
OR with inputs 0 1 gives output 1
```
                ░                 ░    
q_0: ─|0>───────░───■─────────■───░────
          ┌───┐ ░   │         │   ░    
q_1: ─|0>─┤ X ├─░───┼────■────■───░────
          └───┘ ░ ┌─┴─┐┌─┴─┐┌─┴─┐ ░ ┌─┐
q_2: ─|0>───────░─┤ X ├┤ X ├┤ X ├─░─┤M├
                ░ └───┘└───┘└───┘ ░ └╥┘
c: 1/════════════════════════════════╩═
                                     0 
```
OR with inputs 1 0 gives output 1
```
          ┌───┐ ░                 ░    
q_0: ─|0>─┤ X ├─░───■─────────■───░────
          └───┘ ░   │         │   ░    
q_1: ─|0>───────░───┼────■────■───░────
                ░ ┌─┴─┐┌─┴─┐┌─┴─┐ ░ ┌─┐
q_2: ─|0>───────░─┤ X ├┤ X ├┤ X ├─░─┤M├
                ░ └───┘└───┘└───┘ ░ └╥┘
c: 1/════════════════════════════════╩═
                                     0 
```
OR with inputs 1 1 gives output 1
```
          ┌───┐ ░                 ░    
q_0: ─|0>─┤ X ├─░───■─────────■───░────
          ├───┤ ░   │         │   ░    
q_1: ─|0>─┤ X ├─░───┼────■────■───░────
          └───┘ ░ ┌─┴─┐┌─┴─┐┌─┴─┐ ░ ┌─┐
q_2: ─|0>───────░─┤ X ├┤ X ├┤ X ├─░─┤M├
                ░ └───┘└───┘└───┘ ░ └╥┘
c: 1/════════════════════════════════╩═
                                     0 
```
