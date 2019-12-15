### Appendix E. Lagrange Multipliers.

Lagrange multipliers는 constraint 가 여러개 있는 함수의 stationary points  찾기위해 사용된다.

 이런식으로 생긴 constraint를 갖는 함수  의 최대값을 구하는 문제를 생각해보자

푸는법 1번 constraint equation, express  를  에대한 식으로 표현, .

결국 이렇게 다시 표현 가능 .

The maximum with respect to  일반적인 방법으로 미분해서 얻을 수 있다.

stationary value  를 얻으면,  를 이렇게 표현해 .

이렇게 풀면 해석적 solution인   에 대한 함수로 표현한  를 찾기가 어려워

또한, 이렇게 풀면  를 각각 풀기 때문에 자연스러운 대칭성을 저해한다.

그래서 멋지고 간단하게 Lagrange multiplier  를 사용해서 풀어. 기하학적 관점에서 나온거긴 해.

D 차원의 변수들을 생각해보자 . ![Screen Shot 2019-12-03 at 2.27.01 PM](file:///Users/choi/Desktop/Screen%20Shot%202019-12-03%20at%202.27.01%20PM.png?lastModify=1575352887)

그림처럼, constraint equation  는 n-1차원의 surface를 형성한다.

The gradient  위에 있는 모든 점이 surface에대해 수직인걸 알수 있다.

A point x 가 surface위에 있고, nearby point   또한 surface 위에 있다는걸 생각해야해

x 주변 점에대해 Taylor 전개를 하면,  가 된다. 

x and  둘다 constraint surface위에 있기 때문에,  이고   이다.

In the limit  we have , and because  is then parallel to the constraint surface , we see that the vector  is normal to the surface.

Next  point  를 찾겠다 on the constraint surface such that f(x) is maximized.

이러한 점들은 반드시 그림처럼, the vector  is also orthogonal to the constraint surface, 그렇지 않으면  의 value를 constraint surface 를 따라 약간 움직이면 증가시킬수 있기 때문이다.

그러므로  는 0도 혹은 180도 의 벡터이다. 그리고 parameter  를 반드시 갖는다. Such that  

Where  is known as a Lagrange multiplier. Note that  can have either sign.



At this point it is convenient to introduce the Lagrangian function defined by  .

The constrained stationarity condition  is obtained by setting  

Furthermore, the condition  leads to the constraint equation  .

Thus to find the maximum of a function  subject to the constraint , 

We define the Lagrangian function given by  .and we then find the stationary point of  with respect to both x and  . 

For a D-dimensional vector x, this gives D+1 equations that determine both the stationary point  and the value of . 

If we are only interested in , then we can eliminate  from the stationarity equations without needing to find its value (hence the term 'undetermined multiplier').

As a simple example, suppose we wish to find the stationary point of the function  subject to the constraint , as illustrated in Figure. 

![Screen Shot 2019-12-03 at 2.45.13 PM](file:///Users/choi/Desktop/Screen%20Shot%202019-12-03%20at%202.45.13%20PM.png?lastModify=1575352887)

The corresponding Lagrangian function is given by  

The conditions for this Lagrangian to be stationary with respect to  give the following copied equations:



Solution of these equations then gives the stationary point as  , and the corresponding value for the Lagrange multiplier is  

So far, we have considered the problem of maximizing a function subject to an equality constraint of the form  

We now consider the problem of maximizing f(x) subject to an inequality constraint of the form , as illustrated in Figure

![Screen Shot 2019-12-03 at 2.50.10 PM](file:///Users/choi/Desktop/Screen%20Shot%202019-12-03%20at%202.50.10%20PM.png?lastModify=1575352887)

There are now tow kinds of solution possible, according to whether the constrained stationary point lies in the region where , in which case the constraint is inactive, or whether it lies on the boundary , in which case the constraint is said to be active.

In the former case, the function g(x) plays no role and so the stationary condition is simply . 

This again corresponds to a stationary point of the Lagrange function but this time with .

The latter case, where the solution lies on the boundary, is analogous to the equality constraint discussed previously and corresponds to a stationary point of the Lagrange function with .

Now, however, the sign of the Lagrange multiplier is crucial, because the function f(x) will only be at a maximum if its gradient is oriented away from the region g(x) >0, as in figure.

We therefore have  for some value of .

For either of these two cases, the product .

Thus the solution to the problem of maximizing f(x) subject to g(x) 0 is obtained by optimizing the Lagrange function with respect to x and  subject to the conditions



These are known as the KKT condition.

Note that if we wish to minimize the function f(x) subject to an inequality constraint g(x)  0, then we minimize the Lagrangian function  with respect to x , again subject to .

Finally, it is straightforward to extend the technique of Lagrange multipliers to the case of multiple equality and inequality constraints.

Suppose we with to maximize f(x) subject to 

We then introduce Lagrange multipliers {} and { }, and then optimize the Lagrangian functnio given by

  

Subject to  and  for .

Extensions to constrained functional derivatives are similarly straight forward.