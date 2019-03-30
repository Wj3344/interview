# 重点：
- hashCode() 用于散列集合的查找
- equals() 用于判断两个对象是否相等

- hashCode()和equals()之间的关系

    1、如果两个对象相同（即用equals比较返回true），那么它们的hashCode值一定要相同
    
    2、如果两个对象的hashCode相同，它们并不一定相同(即用equals比较返回false)
    
Java中的HashMap使用hashCode()和equals()方法来确定键值对的索引，当根据键获取值的时候也会用到这两个方法。如果没有正确的实现这两个方法，两个不同的键可能会有相同的hash值，因此，可能会被集合认为是相等的。而且，这两个方法也用来发现重复元素。所以这两个方法的实现对HashMap的精确性和正确性是至关重要的。