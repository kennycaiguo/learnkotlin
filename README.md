# learnkotlin
# 第一个kotlin程序
fun main(args:Array<String>){
    println("Hello kotlin")
     
}

# kotlin中声明函数已经字符串模板的使用
fun main(args:Array<String>){
    println("Hello kotlin")
    var x=10
    var y=20
 
   println("$x+$y=${add(x,y)}")//注意在kotlin中，println函数只有一个参数，所以要使用字符串模板
}

fun add(x:Int,y:Int):Int{
    return x + y
}

# kotlin中使用可变参数
fun main(args:Array<String>){
    println("a+...=${anySum(11,22,33,44)}")//注意在kotlin中，println函数只有一个参数，所以要使用字符串模板
}

 

fun anySum(vararg nums:Int):Int{ //kotlin中可变参数用vararg来声明
    var sum:Int =0;
    for(num in nums){
        sum+=num
    }
    return sum
}
# kotlin中使用lambda表达式
## 实例1
fun main(args: Array<String>) {
    val sumLambda: (Int, Int) -> Int = {x,y -> x+y}
    println(sumLambda(1,2))  // 输出 3
}

##   实例2
fun main(args:Array<String>){
    println(lambdaAdd(10,20))
    
}

fun lambdaAdd(a:Int,b:Int):Int{
    val add:(Int,Int)->Int={x,y->x+y} //lambda表达式的使用
    return add(a,b)
}
    
