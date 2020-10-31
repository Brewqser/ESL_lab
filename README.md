# ESL_lab
Tutorials done for ESL laboratories.

### Content

Each tutorial has its own folder in whitch u can find:
* python script (written in jupyter notebook)
* generated verilog (only final file used to created bitstream)
* bitstream implementations (as Vivado 2020.1 archive file)

### Problems
There was only one problem with all tutorials.
In tutorial "Hierarchy and Abstraction and Ursidae, Oh My!" genereted file had following error
```
[Synth 8-1031] None is not declared ["E:/semestr7/ESL/Tutoriale/ESL_lab/2_Hierarchy/blinker.v":159]
```
To fix this I needed to change line 159 in blinker.v
```
assign k_chunk_insts_0_chunk_insts_6_chunk_insts_0_a[0] = Nope;
```
to
```
assign k_chunk_insts_0_chunk_insts_6_chunk_insts_0_a[0] = 0;
```
