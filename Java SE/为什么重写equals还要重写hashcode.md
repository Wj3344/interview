# 重点：
- hashCode() 用于散列集合的查找
- equals() 用于判断两个对象是否相等

- hashCode()和equals()之间的关系

    1、如果两个对象相同（即用equals比较返回true），那么它们的hashCode值一定要相同
    
    2、如果两个对象的hashCode相同，它们并不一定相同(即用equals比较返回false)