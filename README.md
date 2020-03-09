exp4j
-----
exp4j is a mathematical expression evaluator for the Java programming language. It is a simple-to-use and small library (~50kb) without any external dependencies.

Check out http://www.objecthunter.net/exp4j/ for documentation and examples


## 简介
    Exp4j是一个简单易用的开源Java数学表达式计算工具，由德国Java开源爱好者Frank发起并持续进行维护，旨在提供对数学表达式的计算功能。

## 使用
    Expression e = new ExpressionBuilder("3 * (sin(pi) - 2 )/ e")
        .variables("pi", "e")
        .build()
        .setVariable("pi", Math.PI)
        .setVariable("e", Math.E);
    double result = e.evaluate();


## pom
    <dependency>
        <groupId>net.objecthunter</groupId>
        <artifactId>exp4j</artifactId>
        <version>0.4.8</version>
    </dependency>

## 表达式变量定义
- 变量的定义可以使用字母、汉字、下划线、数字，但是不能以数字开头。

## Exp4j所支持的运算符包括：
- 加法：“2 + 2”
- 减法：“2 - 2”
- 乘法：“2 * 2”  
- 除法：“2 / 2”
- 取模：“2 ％ 2”
- 正负号：“+2 - (-2)”
- 幂：“2 ^ 2”

## 内置函数
- sqrt(身高)  开方
- abs: absolute value
- acos: arc cosine
- asin: arc sine
- atan: arc tangent
- cbrt: cubic root
- ceil: nearest upper integer
- cos: cosine
- cosh: hyperbolic cosine
- exp: euler's number raised to the power (e^x)
- floor: nearest lower integer
- log: logarithmus naturalis (base e)
- sin: sine
- sinh: hyperbolic sine
- sqrt: square root
- tan: tangent
- tanh: hyperbolic tangent

## 表达式样例
- 3 * sin(y) - 2 / (x - 2)
- 3log(y)/(x+1)
- 2cos(xy)
- 2*Math.PI + Math.E
- pi+π+e+φ
- 7.2973525698e-3

## 官网
https://www.objecthunter.net/exp4j/
