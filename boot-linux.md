#### 主引导记录

- 1 - 446字节（共446字节）：机器码
- 447 - 510字节（共64字节）：分区表
- 511、512字节：主引导记录（0x55和0xAA）

#### 分区表

- 64字节的分区表分为四个部分（主分区），每个部分16字节
- 第1个字节：0x80表示激活的主分区
- 第2 - 4字节：主分区第一个扇区的物理位置
- 第5个字节：主分区类型
- 第6 - 8字节：主分区最后一个扇区的物理位置
- 第9 - 12字节：主分区第一个扇区的逻辑地址
- 第13 - 16字节：主分区的扇区总数
- 有且仅有一个区可以被定义为扩展分区