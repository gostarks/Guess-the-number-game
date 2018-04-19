# Guess-the-number-game
import java.util.*

fun main(args: Array<String>) {
    println("Do you wan to play a game")
    var q:String=readLine()!!
    if(q=="yes"){
        do{
            val random=Random()
            var a=random.nextInt(5)
            println("Guess the number between 0-5")
            var b=readLine()!!
            if(a==b.toInt())
            {
                println("Bravo!! you have guess it right")
            }
            else
            {
                println("Wrong , please enter again")
                var b= readLine()!!
                if(a==b.toInt())
                {
                    println("Bravo!! you have guess it right")
                }
                else
                {
                    println("Wrong again , please enter again")
                    var b= readLine()!!
                    if(a==b.toInt())
                    {
                        println("Bravo!! you have guess it right")
                    }
                    else
                    {
                        println("Sorry you have used all your option , the number was $a")
                    }

                }
            }
            println("Do you want to play again")
            q= readLine()!!
        }while(q=="yes")
    }
}
