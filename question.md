    sentence1 = '你和我聊天辛苦吗？'
    # 1	你	你	r	r	_	4	主谓关系	_	_
    # 2	和	和	c	c	_	4	状中结构	_	_
    # 3	我	我	r	r	_	2	介宾关系	_	_
    # 4	聊天	聊天	v	v	_	0	核心关系	_	_
    # 5	辛苦	辛苦	a	a	_	4	动补结构	_	_
    # 6	吗	吗	e	y	_	4	右附加关系	_	_
    # 7	？	？	wp	w	_	4	标点符号	_	_
    
    sentence2 ='和我聊天辛苦吗'
    # 1	和	和	c	c	_	3	状中结构	_	_
    # 2	我	我	r	r	_	1	介宾关系	_	_
    # 3	聊天	聊天	v	v	_	0	核心关系	_	_
    # 4	辛苦	辛苦	a	a	_	3	动补结构	_	_
    # 5	吗	吗	e	y	_	3	右附加关系	_	_

    sentence3 = '你可以和我聊天吗？'
    # 1	你	你	r	r	_	5	主谓关系	_	_
    # 2	可以	可以	v	v	_	5	状中结构	_	_
    # 3	和	和	p	p	_	5	状中结构	_	_
    # 4	我	我	r	r	_	3	介宾关系	_	_
    # 5	聊天	聊天	v	v	_	0	核心关系	_	_
    # 6	吗	吗	e	y	_	5	右附加关系	_	_
    # 7	？	？	wp	w	_	5	标点符号	_	_
    
    sentence4 = '我想和你聊天'
    # 1	我	我	r	r	_	2	主谓关系	_	_
    # 2	想	想	v	v	_	0	核心关系	_	_
    # 3	和	和	p	p	_	5	状中结构	_	_
    # 4	你	你	r	r	_	3	介宾关系	_	_
    # 5	聊天	聊天	v	v	_	2	动宾关系	_	_
    

含义相同的句子，句法却大不相同:    
sentence3 实际最相似的是 sentence4 
sentence3 句法最相似的是 sentence1
sentence2 缺少主语

sentence = '你是谁造的'
sentence = '谁造出你的'

=spoken language=: 1-补全缺省部分，2-移除可缺省的部分，3-提取核心词语

    
0-人称代词 - 
0 - ques         含/不含代词  ->  (主语省略)-代词恢复
1 - toplist_ques 含/不含代词  ->  (主语省略)-代词恢复


其他问题：
'小M，知道我是谁吗' - 称呼
'你好你在干什么' - 省略标点
'你的性别是' - 省略'什么'


要解决的问题是什么？
1，机器人搞不清对象（你我他）
2，句向量匹配检索结果有问题 - 针对返回结果再次过滤  -  关键词提取算法？

