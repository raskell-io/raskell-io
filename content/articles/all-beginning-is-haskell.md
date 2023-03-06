---
title: "All beginning is Haskell"
author: "Raffael"
date: "2023-03-06"
description: "All beginning is Haskell"
tags:
- haskell
categories:
- code
katex: true
---

![all-beginning-is-haskell.png](all-beginning-is-haskell.png)

## The beauty of mathematics

Mathematics is often considered beautiful because it provides a way to describe and understand the world in a way that is precise, elegant, and abstract. Mathematics can be seen as a language that allows us to describe complex phenomena and patterns in a way that is independent of the particular objects or situations involved. This abstract quality of mathematics is what makes it so powerful and beautiful.

Mathematics can also be considered beautiful because of its ability to reveal unexpected connections and relationships between seemingly disparate areas of study. By using the language of mathematics to describe complex phenomena, we are able to identify deep and fundamental connections between seemingly unrelated areas of study, revealing the underlying structure and order in the natural world.

As someone who always was drawn by this type of mathematical beauty, I also was naturally drawn to Haskell due to its roots in mathematical theory since the first time I read about Haskell. Haskell was created by a group of researchers who were interested in creating a language that was as pure as possible. The language was designed to be purely functional, meaning that all computations are performed through the evaluation of functions. This approach allows Haskell programs to be more concise and easier to reason about than programs written in imperative languages like Java or C++. As a language that emphasizes purity and immutability, Haskell is particularly well-suited to applications in mathematics, data analysis, and other areas where correctness and maintainability are critical.

In addition to its mathematical roots, Haskell's focus on purity and immutability also appealed to me as a programmer. As someone who has worked on projects with large codebases, I understand the importance of maintainability and the challenges that can arise when code is difficult to reason about or modify. By focusing on pure functions and immutability, Haskell reduces the potential for bugs and makes it easier to modify code without introducing new problems.

In this blog post, I will provide an introduction to Haskell and explore how its focus on pure functions and easy refactoring can make code maintenance easier. I'll also provide some interesting code snippets to help illustrate Haskell's unique approach to programming. Whether you're a seasoned developer or a math enthusiast like myself, I hope that this post will give you a deeper appreciation for the beauty and power of Haskell.

## Mister Curry Haskell

Haskell is named after the logician Haskell Curry, who was a pioneer in the field of mathematical logic and contributed significantly to the development of the lambda calculus. The lambda calculus is a mathematical notation system for expressing computation that is closely related to functional programming.

Haskell was developed in the late 1980s by a group of researchers, including Simon Peyton Jones, Philip Wadler, and others, who were interested in creating a purely functional programming language that was inspired by the lambda calculus. They named the language after Haskell Curry as a tribute to his contributions to mathematical logic.

Haskell's focus on purity and immutability is closely related to the lambda calculus, which is based on the idea of functions as first-class citizens. In Haskell, functions are treated as values that can be passed around, composed, and evaluated just like any other data type. This approach allows Haskell programs to be more concise and easier to reason about than programs written in imperative languages like Java or C++.

Haskell also incorporates many features from other functional programming languages like ML and Lisp, as well as concepts from category theory and other branches of mathematics. The language's sophisticated type system, which includes type inference, type classes, and higher-kinded types, is one of its most distinctive and powerful features.

## The Lambda is the new Alpha

Haskell is closely related to the lambda calculus, which is a mathematical notation system for expressing computation. The lambda calculus was developed in the early 20th century by mathematician Alonzo Church as a way to formalize the notion of computability.

The lambda calculus consists of three basic elements: variables, functions, and applications. Variables represent values, functions represent computations, and applications represent the act of applying a function to an argument. For example, the function $ f(x) = x + 1 $ could be represented in the lambda calculus as the expression $ (λx.x + 1) $ .

Haskell was developed in the late 1980s by a group of researchers, including Simon Peyton Jones, Philip Wadler, and others, who were interested in creating a purely functional programming language that was inspired by the lambda calculus. As mentioned above, they named the language after Haskell Curry as a tribute to his contributions to mathematical logic.

Like the lambda calculus, Haskell is based on the principles of functional programming, which emphasize the use of pure functions and immutable data structures. In Haskell, functions are first-class citizens that can be passed around and composed just like any other data type. This allows Haskell programmers to create powerful abstractions and write code that is more modular and reusable than in imperative languages like C++ or Java.

Haskell's type system is also inspired by the lambda calculus, and includes features like type inference, type classes, and higher-kinded types. This allows Haskell programmers to write code that is both statically typed and expressive, reducing the potential for errors while still allowing for elegant and concise code.

Here's an example of a lambda calculus expression that represents the addition of two numbers:

$$ (λx.λy.x + y) $$

In this expression, λx represents a function that takes an input x, and λy represents a function that takes an input y. The expression x + y represents the sum of x and y.

To use this expression to add two numbers, we apply it to two arguments:

$$ (λx.λy.x + y) 3 4 $$

In this case, the expression is applied to the arguments 3 and 4, resulting in the following computation:

$$ (λy.3 + y) 4 $$

In this expression, the function λx has been replaced with the value 3, resulting in a new function that takes an input y and adds it to 3. This function is then applied to the argument 4, resulting in the value 7.

This example demonstrates the basic principles of the lambda calculus, where functions are used to represent computations and can be composed and applied in a way that is similar to arithmetic operations. These principles form the basis of functional programming, and have been influential in the development of languages like Haskell, which was designed to be closely aligned with the lambda calculus.

## One Type System to rule them all

ML (Meta Language) is considered a precursor to Haskell because it is a functional programming language that shares many of the same concepts and ideas. Like Haskell, ML is strongly typed and supports type inference, pattern matching, and higher-order functions. ML was developed in the 1970s by Robin Milner and others as a tool for writing software that could reason about mathematical objects and proofs. It was initially designed as a metalanguage for describing programming languages, but quickly evolved into a full-fledged programming language in its own right.

One of the key features of ML that influenced the development of Haskell is its support for algebraic data types. Algebraic data types allow programmers to define complex data structures by combining simpler types in various ways, using constructs like sums, products, and variants. This allows for a high degree of expressiveness and modularity in programming. Haskell also inherits many other features from ML, such as its focus on purity, immutability, and higher-order functions. ML also introduced the concept of type inference, which allows type information to be inferred automatically from the code, reducing the need for explicit type annotations.

Haskell's type system is based on the Hindley-Milner type system, which was first introduced in the ML programming language in the 1970s. The Hindley-Milner type system is a type inference algorithm that can deduce the types of expressions in a program without the need for explicit type annotations. In Haskell, the Hindley-Milner type system has been extended and refined to include additional features such as type classes, higher-kinded types, and generalized algebraic data types. These extensions make Haskell's type system more expressive and flexible than the original Hindley-Milner type system in ML.

Type classes are a key feature of Haskell's type system that allow programmers to define common behavior for a set of types. For example, the `Eq` type class defines the notion of equality for a given type, while the Ord type class defines the notion of order. Type classes provide a powerful mechanism for creating modular and reusable code.

Higher-kinded types are another extension to Haskell's type system that allow for more complex and abstract types. In essence, higher-kinded types are types that take other types as arguments, allowing for a greater degree of generality and abstraction in programming.

Generalized algebraic data types (GADTs) are a further refinement of algebraic data types that allow for more precise control over the types of data in a program. GADTs allow programmers to specify more specific constraints on the types of data that can be manipulated, leading to more robust and maintainable code.

Haskell's type system builds on the foundations laid by the Hindley-Milner type system in ML, but extends and refines it to include additional features that make Haskell's type system more expressive and flexible. By providing a powerful and expressive type system, Haskell makes it easier for programmers to write correct and maintainable code.

## ELI5: What is Haskell again?

Haskell is a functional programming language that was first developed in the late 1980s. It is named after the logician Haskell Curry and is designed to be purely functional, meaning that all computations are performed through the evaluation of functions. This approach allows Haskell programs to be more concise and easier to reason about than programs written in imperative languages like Java or C++.

Haskell is a statically-typed language, which means that the type of every expression is known at compile time. This allows the compiler to catch many errors before the program is even run, making it easier to write correct code. Haskell also has a sophisticated type system that allows for powerful abstractions and code reuse.

One of the most distinctive features of Haskell is its laziness. This means that expressions are only evaluated when they are needed, allowing for efficient use of resources and the creation of infinite data structures.

## Getting started with Haskell

To get started with Haskell, you'll need to install the GHC compiler and an editor or IDE that supports Haskell development. Once you have these tools set up, you can start writing Haskell code!

Let's start with a simple "Hello, world!" program:

```haskell
main :: IO ()
main = putStrLn "Hello, world!"
```

This program defines a main function that prints the string "Hello, world!" to the console. The :: operator is used to specify the type of the main function, which in this case is IO (). The IO type represents actions that interact with the outside world, like reading from or writing to files.

## From pure functions to easy refactoring

One of the key benefits of Haskell's functional programming paradigm is that it makes it easy to write pure functions. A pure function is one that has no side effects and always returns the same result given the same input. This property makes pure functions easy to reason about and test.

Let's look at an example. Suppose we have a function that calculates the factorial of a number:

```haskell
factorial :: Integer -> Integer
factorial n = product [1..n]
```

This function takes an Integer and returns its factorial. We can use it like this:

```haskell
> factorial 5
120
```

Now suppose we want to optimize this function by memoizing the results. We can do this easily by using Haskell's memoize function:

```haskell
import Data.Function.Memoize (memoize)

factorial :: Integer -> Integer
factorial = memoize go
  where
    go 0 = 1
    go n = n * factorial (n - 1)
```

The memoize function takes a function and returns a memoized version of it. This means that the function's results are cached for future calls with the same arguments, improving performance.

Note that we didn't need to change any of the code that calls the factorial function. This is because the function's type signature didn't change, and its behavior is still the same. This is an example of how easy refactoring can be in Haskell. By focusing on pure functions and immutability, Haskell makes it easy to modify code without introducing bugs or breaking existing functionality.

The absence of side effects and the use of pure functions can greatly aid in reasoning about code. By eliminating side effects and enforcing purity, it becomes much easier to reason about the behavior of a program and to understand its logic.

Here are some ways in which pure functions and the absence of side effects help with reasoning about code:

- Predictability: Since pure functions do not have side effects, their behavior is entirely determined by their inputs. This makes it easy to predict the output of a pure function given a particular input, making it easier to reason about the behavior of the program as a whole.

- Testability: Pure functions are easy to test because their behavior is entirely determined by their inputs. This makes it easy to write automated tests for pure functions, ensuring that they behave correctly and that any changes to their behavior can be caught early on.

- Modularity: Pure functions are highly modular because they can be composed and reused in a variety of ways. Since they do not have side effects, they can be combined and used in a wide range of contexts without introducing unexpected behavior or side effects.

- Reasoning about state: Pure functions make it easy to reason about the state of a program because they do not modify state. This makes it easier to understand the flow of data through a program and to reason about the relationships between different parts of the program.

The absence of side effects and the use of pure functions can greatly aid in reasoning about code by making it more predictable, testable, modular, and easier to understand. By enforcing purity and avoiding side effects, functional programming languages like Haskell can make it easier to reason about the behavior of complex programs, leading to more robust and maintainable code.

The use of pure functions and the absence of side effects can greatly improve the refactoring potential and code maintainability of a program.

Refactoring is the process of changing the structure of a program without changing its behavior. This can involve adding new features, improving performance, or making the code more modular and reusable. By using pure functions and avoiding side effects, it becomes much easier to refactor a program without introducing unexpected behavior or breaking existing functionality.

By using pure functions and avoiding side effects, functional programming languages like Haskell make it easier to refactor code without introducing bugs or unintended behavior. This improves code maintainability by making it easier to modify and update the codebase over time, reducing the risk of introducing new bugs or breaking existing functionality.

## Purity as a design goal

Pure functions are functions that have no side effects and always return the same result given the same input. In other words, a pure function's output only depends on its input, and it doesn't modify any external state or perform any I/O operations.

This property is desirable for several reasons. First, pure functions are easier to reason about and test. Because they have no side effects, they always produce the same output given the same input, which makes them predictable and easier to verify. This can be especially important in mathematical or scientific contexts where correctness is critical.

Second, pure functions can be composed more easily than impure functions. Because pure functions have no side effects, they can be combined or nested in any order without affecting the final result. This makes it easier to write modular and reusable code that can be composed from smaller building blocks.

Third, pure functions can be more efficient than impure functions in certain contexts. Because pure functions are referentially transparent, meaning that their results depend only on their inputs, they can be memoized or cached to improve performance. This can be especially useful in recursive algorithms or in situations where expensive computations need to be repeated many times.

The concept of pure functions is closely related to mathematical theory, particularly the notion of functions in mathematical analysis.

In mathematics, a function is a mapping between two sets, where each element of the first set is associated with a unique element of the second set. For example, the function f(x) = x^2 is a mapping from the set of real numbers to the set of non-negative real numbers. Given any real number x, the function f(x) returns the square of that number.

Functions in mathematics are often defined in terms of their inputs and outputs, without reference to any external state or context. This is similar to the concept of pure functions in programming, which have no side effects and depend only on their input parameters.

The concept of referential transparency, which is central to the idea of pure functions in programming, also has a mathematical counterpart. In mathematical analysis, a function is said to be referentially transparent if it can be replaced by its value without changing the outcome of any other computations. For example, the function f(x) = x + 1 is referentially transparent, because it can be replaced by its value without affecting the outcome of any other computations.

The use of pure functions in programming can be seen as an extension of these mathematical concepts to the realm of software engineering. By designing programs in terms of pure functions, we can create software systems that are easier to reason about and test, more modular and reusable, and more efficient in certain contexts. This can lead to more robust and maintainable software systems that are better suited to the demands of modern computing.

## The side-effects of functional purity

The concepts of immutability, statelessness, higher-order functions, and lazy evaluation are closely related to the idea of pure functions in programming and are highly prominent in the advantages of a programming language like Haskell. By embracing these concepts, we can create software systems that are more robust, efficient, and maintainable.

- **Immutability**: Immutability is the concept of not modifying data once it has been created. Immutable data structures are often used in functional programming, because they can make it easier to reason about the behavior of a program. In Haskell, many of the built-in data structures are immutable, including lists, tuples, and sets.

- **Statelessness**: Statelessness refers to the concept of not maintaining any internal state between function calls. In other words, a stateless function depends only on its input parameters and has no side effects. Stateless functions are often used in functional programming, because they can make it easier to reason about the behavior of a program.

- **Higher-order functions**: Higher-order functions are functions that take other functions as input parameters or return functions as output. Higher-order functions are often used in functional programming to create powerful abstractions and compose smaller functions into larger ones.

- **Lazy evaluation**: Lazy evaluation is the concept of delaying the evaluation of an expression until it is actually needed. In Haskell, expressions are evaluated only when their values are required to compute the final result of a program. This can lead to more efficient code, because expressions that are not needed are never evaluated.

All of these concepts are closely related to pure functions, because they help enforce the properties of purity and immutability. By using immutable data structures and stateless functions, we can reduce the potential for side effects and create code that is more predictable and easier to reason about. Higher-order functions and lazy evaluation can also lead to more efficient and maintainable code by creating powerful abstractions and reducing the amount of unnecessary computation.

## Nomad as monad

In a purely functional language like Haskell, functions that produce side effects like input/output, state mutation, and exceptions are generally not considered pure. This is because they have the potential to produce different results for the same input, depending on the context in which they are executed.

To work with these effects in a purely functional way, Haskell uses monads to encapsulate the side effects and provide a way to compose and sequence them in a predictable way. For example, the IO monad is used to represent input/output operations, while the State monad is used to represent stateful computations.

In the case of the IO monad, the monadic structure allows the input/output operations to be performed in a predictable and composable way. The IO monad provides functions like >>= (pronounced "bind") and >> (pronounced "then") that allow input/output operations to be sequenced and composed in a way that ensures their order of execution is well-defined.

Similarly, the State monad provides a way to model stateful computations in a pure way. The State monad allows a function to compute a new state value based on an existing state value, without modifying the existing state value. This allows the state to be propagated through a series of function calls in a predictable and composable way.

Monads are therefore a fundamental concept in Haskell and are used to encapsulate effects, such as input/output or state changes, in a purely functional way. Let's take a look at a simple example that demonstrates the use of a monad in Haskell:

```haskell
import Control.Monad.State

-- Define a function that uses the State monad to keep track of a counter
count :: State Int Int
count = do
  n <- get
  put (n + 1)
  return n

-- Use the count function to increment a counter and retrieve its value
result :: Int
result = evalState count 0
```

In this example, we use the State monad to keep track of a counter. The State monad encapsulates stateful computations in a purely functional way, allowing us to write code that has side effects while still adhering to Haskell's purity and immutability.

The count function uses the State monad to read the current value of the counter, increment it by 1, and return its original value. This is achieved using the get, put, and return functions provided by the State monad.

The result variable uses the evalState function to run the count function with an initial state of 0. This results in the counter being incremented by 1 and its value being returned, which is then assigned to the result variable.

This example demonstrates how monads can be used to encapsulate side effects in a purely functional way, making it easier to reason about and maintain code. The State monad is just one example of a monad in Haskell, and there are many others, such as the IO monad for input/output operations and the Maybe monad for handling optional values.

By using monads, Haskell programmers can write code that has side effects in a way that is consistent with the language's focus on purity and immutability. This can lead to more robust and maintainable software systems that are easier to test and modify over time.

In mathematics, a monad is a structure that describes a certain kind of algebraic operation. Specifically, a monad is a triple (T, η, μ) consisting of:

- A functor T that maps a category C to itself. This functor is often called the "monad functor".
- A natural transformation η from the identity functor on C to T. This natural transformation is called the "unit" of the monad.
- A natural transformation μ from T∘T to T. This natural transformation is called the "multiplication" of the monad.
The monad structure is used in mathematics to describe a wide range of mathematical structures and operations, including algebraic structures like groups, rings, and fields, as well as more abstract structures like topological spaces and sheaves.

In computer science, monads are used as a programming construct that provides a way to encapsulate computation and control side effects in a purely functional way. In this context, a monad is typically defined as a type constructor that provides a way to combine and sequence operations in a way that is both composable and predictable. Monads are often used in functional programming languages like Haskell to model a wide range of effects, including input/output, state, and exceptions.

## Why everyone should learn a Haskell for a great good

One of the benefits of learning Haskell is that it can help you develop a deeper understanding of programming concepts like recursion, higher-order functions, and lazy evaluation. Haskell's focus on purity and immutability can also help you develop good programming habits that can be applied to other languages.

However, despite its many advantages, Haskell is not as commonly used as other programming languages like Java or Python. This is due in part to its steep learning curve and the fact that it is less widely taught in universities and other educational institutions. Haskell also has a smaller community of developers than some other languages, which can make it harder to find resources and support.

Despite these challenges, there are many reasons to learn and use Haskell. For example, Haskell's focus on purity and immutability can lead to more robust and maintainable code. The language's type system can also catch many errors at compile time, reducing the potential for bugs. In addition, Haskell's focus on functional programming can help you develop good programming habits that can be applied to other languages. Here are some of the reasons why it is worthwhile to learn Haskell:

- Learning Haskell can help you develop a deeper understanding of programming concepts like recursion, higher-order functions, and lazy evaluation. Haskell's focus on purity and immutability can also help you develop good programming habits that can be applied to other languages.
- Haskell's sophisticated type system can catch many errors at compile time, reducing the potential for bugs. This can lead to more robust and maintainable code.
- Haskell's focus on purity and immutability can lead to more elegant and concise code that is easier to reason about and test.
- Haskell is a powerful tool for data analysis, machine learning, and other computational tasks that involve complex algorithms and mathematical models.
- Haskell has a small but passionate community of developers who are constantly pushing the boundaries of what is possible with functional programming.

## Conclusion

One of the key benefits of Haskell's functional programming paradigm is that it makes it easy to write maintainable code. By focusing on pure functions and immutability, Haskell reduces the potential for bugs and makes it easier to modify code without introducing new problems.

The use of pure functions means that code is easier to reason about and test. Pure functions have no side effects and always return the same result given the same input. This property makes them easy to test and reduces the potential for bugs. In addition, pure functions are composable, meaning that they can be combined to create more complex functions. This allows for the creation of highly modular and reusable code, which can simplify the process of maintaining and updating code over time.

Haskell's emphasis on immutability also contributes to code maintainability. Immutable data structures are less prone to bugs and can be easier to reason about than mutable ones. Immutable data structures also encourage a functional style of programming, which can lead to more concise and elegant code.

Ultimately, Haskell's focus on functional programming, immutability, and easy refactoring makes it an ideal choice for building maintainable code. By reducing the potential for bugs and making it easier to modify code over time, Haskell can help developers create software that is robust and easy to maintain.

## References and further reading