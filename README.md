version 1.0 : 完成单周期CPU(24条指令)
version 1.1 : 正在做中断(转去做差异化指令，放弃）
version 1.2 ： 1.2.0版本完成硬布线控制器，经测试修改后不影响其他24条指令的运行；1.2.1版本完成BGEZ,SUBU,XOR；1.2.2版本完成SB；
      加入差异化指令，SUBU在没有设置差异化指令的情况下与SUB的输出信号完全相同；XOR与OR也只有ALU_OP上有差异；BGEZ的输出信号与BEQ也相同，但是由于是与0比较，需要多一个输出信号，命名为BGEZ同时对电       路进行一定改动，而且默认有符号数，ALU_OP取11；SB指令比较复杂，需要将要写入的字节和存储器中本来就有的字节进行拼装再写回
version 1.3 ： 完成理想流水线
       1.3.0版本完成流水接口部件设计，1.3.1完成理想流水线
version 1.4 ： 气泡流水线(EX段分支)
version 1.5 ： 重定向流水线(EX段分支)
       个人感觉1.5版本是正确的，但是1.5-TEXT 版本才可以通过提交
version 1.6 ： 单级中断
