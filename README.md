# OnePiece.github.io
#Redis学习笔记
#This is my personal blog.
一 Redis数据类型
1.	SDS 
Redis自构建一个简单动态字符串SDS
      定义为：struct sdshdr{
							Int len;
							Int free;
                   Char buf[ ];//保存二进制数据 可以保存任何二进制数据，数据没有限制
};
优点：1.常数复杂度获取字符串长度
2.杜绝缓冲区溢出
3.减少修改字符串时带来的内存重分配次数
 
 
2.链表
