## 3.6 MongoDB建模分析

1：将用户信息集合与收藏记录集合、转发记录集合做成内嵌关系，即用户集合中包含收场记录和转发记录两个集合。  

2：将我的关注集合作为一个独立的集合，因为该集合涉及到关注人和被关注人两项关键数据，在表达关注人的信息时无法表达被关注人的信息。如果作两个内嵌，这样冗余数据特别多，无法清晰表现。  

3：将用户集合与博文集合之间采用引用关系。该引用采用用户名进行直接引用。  

4：博文与评论之间采用一对多的内嵌式关系。  

5：关键点在于转发信息会内嵌于用户集合和博文集合两个集合中，属于冗余数据。
