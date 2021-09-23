# JVM

類加載 (類初始化)：分三步驟，加載，連接，以及初始化過程

方法區
常量池
元數據
永久

constant_pool table 是用來產生 run-time constant pool

## ClassLoader

類加載器的輸入是類文件(Hello.class) 輸出有兩個
第一個是是類物件(Hello Class Object) 存在堆裡
第二個是類別的各種資訊 比如說字段名稱描述符 方法名稱描述符等等 存在方法區

類加載時機
分為主動使用以及被動使用
主動使用：主動使用一個類別，代表需要初始化，要初始化之前必須要經過加載的步驟
被動使用：類別會被加載，但是不會被初始化

主動使用：
- new
- static method 被呼叫
- static variable 被存取 (compile-time 常數不在其中)
- 初始化類別的父類別
- 主類 (public static void main(String[] args) 所在的類)
- 反射的調用
- 

