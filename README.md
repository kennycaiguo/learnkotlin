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
