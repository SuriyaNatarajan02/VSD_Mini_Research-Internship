# TASK-3

 Functional simulation experiment using RISC-V Core Verilog netlist and testbench.
   *  IVERILOG:-Icarus Verilog, commonly referred to as IVerilog, is an open-source Verilog simulation and synthesis tool. It supports a wide range of Verilog standards and is used for designing and testing digital circuits. IVerilog is popular for its flexibility, allowing users to simulate complex designs and generate netlists for various FPGA and ASIC platforms. It is widely used in both educational and professional settings for hardware design and verification.

   *  GTKWAVE:- GTKWave is an open-source waveform viewer used for visualizing simulation results from digital circuit designs. It is commonly used in conjunction with simulation tools like Icarus Verilog.It is a fully featured GTK+ based waveform viewer for Unix and Win32, capable of displaying signal waveforms dumped in a variety of formats.

     
1. INSTALL IVERILOG: using follwing command:-

    $ sudo apt install iverilog 

![Screenshot from 2024-06-02 23-58-19](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/ff7a518d-afc5-4df8-a7d5-2d2d91f1b235)

INSTALL GTKWAVE:
using following command:-

    $ sudo apt install iverilog gtkwave

![Screenshot from 2024-06-02 23-58-05](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/5e8ba270-809f-4ae3-a532-1ad4b5375631)

2. created the verilog file and testbench file in github repository.

cloned it to machine using following command:-

    $ git clone [https://github.com/SuriyaNatarajan02/VSD-Mini-Research-Internship]
    $ cd VSD_Mini_Research_Internship

![Screenshot from 2024-06-02 23-57-57](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/9a36496a-56f4-4691-9e83-cf4ec512f72d)

![Screenshot from 2024-06-02 23-58-28](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/6ae9eff0-5ab2-4d08-a8da-a63607551345)

simulate and run the code ,using following command:-

    $ iverilog -o VSD_Mini_Research_Internship Suriya_rv32i.v Suriya_rv32i_tb.v
    $ ./vsdsquadron-mini-internship

![Screenshot from 2024-06-02 23-58-28](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/6ae9eff0-5ab2-4d08-a8da-a63607551345)

![Screenshot from 2024-06-02 23-58-11](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/fa869c13-e4b6-41f3-b358-344bf14f9776)

And for output waveform give following command:-

    $ gtkwave Suriya_rv32i.vcd

![Screenshot from 2024-06-02 23-58-33](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/cc762584-fe79-4d36-9eab-9e3f7a689490)

3.Analyze the wave form of each instruction using gtkwave.

following instruction are:-
   1.ADD r6, r2, r1
    
   2.SUB r7, r1, r2
    
   3.AND r8, r1, r3
   
   4.OR r9, r2, r5
    
   5.XOR r10, r1, r4
    
   6.SLT r11, r2, r4
    
   7.ADDI r12, r4, 5
    
   8.SW r3, r1, 2
    
   9.SRL r16, r14, r2
    
   10.BEQ r0, r0, 15

Let's analyze:-

    1.ADD r6, r2, r1

![Screenshot from 2024-06-02 23-45-29](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/20628c75-5172-4bb4-9db2-9117ffac2cbf)

   2.SUB r7, r1, r2

![Screenshot from 2024-06-02 23-46-35](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/2b52f3d6-5522-42f7-b9c4-7b5159e31590)   3.AND r8, r1, r3

   3.AND r8, r1, r3

![Screenshot from 2024-06-02 23-46-51](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/b941d4d6-caae-429f-93ef-fca9cd2c45f3)
   
   4.OR r9, r2, r5

![Screenshot from 2024-06-02 23-47-03](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/47ef07ef-7f81-4afa-875e-b704017a0138)
  
  5.XOR r10, r1, r4

![Screenshot from 2024-06-02 23-47-03](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/47ef07ef-7f81-4afa-875e-b704017a0138)
 
  6.SLT r11, r2, r4

![Screenshot from 2024-06-02 23-47-03](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/47ef07ef-7f81-4afa-875e-b704017a0138)
  
  7.ADDI r12, r4, 5

![Screenshot from 2024-06-02 23-47-12](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/c23bc360-dcc1-4bfc-8669-f1b8b5648fea)

   8.SW r3, r1, 2

![Screenshot from 2024-06-02 23-47-28](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/a5ec1fe6-37f8-4246-88a7-a34906b0eaae)

   9.SRL r16, r14, r2

![Screenshot from 2024-06-02 23-47-22](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/95fac7f2-3590-4b45-afb2-ca4293d45307)

   10.BEQ r0, r0, 15

![Screenshot from 2024-06-02 23-46-42](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/f76e6a7a-5778-4e63-b07c-ac865e7364c0)

Full 5-stage instruction pipeline and pc-increment description Waveform

![Screenshot from 2024-06-02 23-46-57](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/80edadc4-5fbb-45f1-bf2f-b1d46002f96c)
