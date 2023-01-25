# Android RoadMap for Interview
Android, Java and Kotlin RoadMap

## [Java](https://github.com/goodluck3301/android-interview/tree/main/Java)
- [x] Java8 vs Kotlin (ex. Data Structure, Why Kotlin?)
- [x] [Java Multithreading](https://github.com/goodluck3301/android-interview/tree/main/Java/MultiThreading)
- [x] Thread Communication
- [x] Memory Managmend (Stack/Heap)
- [x] Garbage Collection
- [x] Extension Methods

## [Kotlin](https://github.com/goodluck3301/android-interview/tree/main/Kotin)
- [x] Data Class
  - [Kotlin Data Class Tutorial with Example](https://www.youtube.com/watch?v=L0VulZZPGbI)
- [x] Data Class vs Class
  - [Kotlin DATA CLASS. Object Oriented Programming in Kotlin for Android #8.10 (Video - EN)](https://www.youtube.com/watch?v=Z6xj7hta7Ac)
- [x] Sealed Classes, Enum Classes, Sealed Interfaces
  - [Sealed Classes](https://medium.com/jesus-medina/sealed-classes-and-sealed-interfaces-advanced-kotlin-a8f6de0c9eaf)
  - [Sealed Classes VS. Enum Classes VS. Sealed Interfaces - When to Use Which?](https://www.youtube.com/watch?v=kLJRZpRhX1o)
- [x] Inline Function
  - In Kotlin, the higher-order functions or lambda expressions, all stored as an object so memory allocation, for both function objects and classes, and virtual calls might introduce runtime overhead. Sometimes we can eliminate the memory overhead by inlining the lambda expression. In order to reduce the memory overhead of such higher-order functions or lambda expressions, we can use the inline keyword which ultimately requests the compiler to not allocate memory and simply copy the inlined code of that function at the calling place.
   ```kt
  fun main(args: Array<String>) {  
      inlineFunction({ println("calling inline functions")})  
  }  
  
  inline fun inlineFunction(myFun: () -> Unit ) {  
    myFun()  
      print("code inside inline function")  
  }  
    ```
   
    ```kt
   fun main(args: Array<String>){
      println("Main function starts")
      inlinedFunc({ println("Lambda expression 1")
      return },      // inlined function allow return
                   // statement in lambda expression
                   // so, does not give compile time error
 
      { println("Lambda expression 2")} )
 
      println("Main function ends")
    }
    
    // inlined function
    inline fun inlinedFunc( lmbd1: () -> Unit, lmbd2: () -> Unit  ) { 
      lmbd1()
      lmbd2()
    }
    ```
- [x] Suspend Function
  - [Suspend Functions - Kotlin Coroutines (Video - En)](https://www.youtube.com/watch?v=yc_WfBp-PdE) 
- [x] Higher-Order Functions and Lambdas in Kotlin
- [x] Infix notation in Kotlin
- [x] Mastering Flow API in Kotlin
- [x] Kotlin Coroutines
- [x] [Data Structure(ex. map, hashMap, list...)](https://github.com/goodluck3301/data-structures-and-algorithms)
- [x] Garbage Collection
- [x] Extension Methods


## [Android](https://github.com/goodluck3301/android-interview/tree/main/Android)

- [x] [Android Components](https://github.com/goodluck3301/android-interview/tree/main/Android#android-components)
- [x] Core Android
- [x] Android Libraries
- [x] Android Architecture
- [x] Android Design Problem
- [x] Android Unit Testing
- [x] Android Tools And Technologies
- [x] Java and Kotlin
- [x] Kotlin Coroutines
- [x] [Multiprocess on Android](https://medium.com/@rotxed/going-multiprocess-on-android-52975ed8863c)
- [x] Kotlin Flow API
- [x] Jetpack Compose
- [x] Other Topics
- [x] Data Structures and Algorithms


### Sites
[Amit Shekhar-Blog (Java/Kotlin/Android)](https://github.com/amitshekhariitbhu/android-interview-questions#core-android)</br>
[Java](https://www.javapedia.net/module/Java)
