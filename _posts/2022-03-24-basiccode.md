---
layout: post
title:  "C & C++ Basic code"
---

# C & C++ Basic code
    //
    /* */
#
    C 
      printf("");
      scanf("%", &);
     C++
      cout << "" << endl;
      std::sin >> "";
# 
    "" in
    %d = number
    %.0f = real num(.num)
    %lf = double
    %e = real num exponential
    %g = law size = f // big size = e
  
    %c = one charter(word)
    %s = sentence
  
    %p = pointer 16bit
    %x = 16bit
    %o = 8bit
#
    Data type - variable(data type name) = value;
      type = char&bool , int , float&double // byte , short , long
      type check = sizeof(type)
      temporarily type change = (type)var
#
    Value Calcution - unsigned(- -> all + // %u)
      literal(print value exp) -- long / longlong // un int / un long // un long / un long long
        ("%ld", L / "%lld", LL) // ("%u", U / "%lu", UL) // ("%lu", UL / "%llu", ULL)
      '+ '- '*
      // (quotient&remainder) - / %  = a/b = b√a
      +=  -=  *=  /=  %/  ++  --  //  var<<num(2^1, 2^2 ---)  var>>num(2^-1, 2^-2 ---)
      >  <  ==  >=  <=  !=  // bit - &  |  !  //  &&  ||
      #include<math.h> -- pow( , ) // sqrt()

#
      if(condition 1) { 1 - true sen }
      elesif(condition 2) {}
      else {all false}

    switch ()
    case n: break
    default:

    x: -- go-to x

#
    while(true condition) {
          true sentence }
    
    do {
      true sentence
    } while(true condition)
    
    for(0~2; true condition; 0~2){
          true sentence }
    
    break; // out of for {}
    continue; // skip 1time to for

#
    Array // [행][열] --  [x][y]  -- 1차원 [y]  --> 2차원 [x][y]로 []는 뒤가 아닌 앞에 
    data type  value[array size];
    if arr size skip => int a[] = { , , , , ... };
    ★ array start = 0 ~ n-1 (n = array size)
    
    n dimension Array
    data type  value[1 dimension array size][2 dim arr size];
    
#
    C String -- <string.h>
    char s[size]; scanf("%s", s);
    strlen(var); // string size
    strcpy(to copy2 , from copy1);
    strcat(var, "+string");
    strcmp(compare1, compare2);

#
    pointer = var address = * | &
    
    /*
        포인터의 * 위치
        int *pit = &a;  ≠ int *pit; *pit=20;
        전자는 초기화    ≠ 후자는 초기화를 했다면 지정 주소의 값 변경
    */
    
    datatype *var = pointing var address; // int *ptr = &arr;
    + **var = another pointer address;   // int **prt_a == *ptr;
    // 기본 포인터는 1차원 배열로 입출력 ∴ 2차원 이상의 접근은 배열-포인터가 필요함
    
    Array - Pointer relationship
    pointer +1(calcution) => datatype as much as change(포인터 +는 주소값의+, 주소값의 크기는 자료형)
      // arr+n은 &arr[0]과 같기에 배열 [1]개의 크기 <-> &arr+n은 배열 [전체]의 크기
      // int *ptr +1 => 00000000 +1 = 00000004  <-> &(*ptr) +1 => 00000000 +1 = 00000012
    
    // *ptr = arr;  arr[i] == *(arr+i) == *(ptr+i) =(교환)= *(i+ptr) == ?? i[ptr]
    
    /*
        arr이라는 배열 변수 이름은 &arr로 변수 자체로 주소값을 가지고 있다.
        (양변에 +i - i는 배열의 번째) arr+i == &arr+i  ==> 이는 배열 주소값으로 i번째의 '주소값'을 찾는다
        
        // (양변에 *추가 - * 값을 인쇄) *(arr+i) ≠ *(&arr+i)  -- 전자는 값 ≠ 후자는 *(&&arr+i)로 주소값을 인쇄
        // 이로인해 프로그램은 arr이라는 배열 자체는 &arr로 변경 후 컴파일러(?)를 예상함
        
        // 추가) 기존에 사용하는 arr[i]는 값이 출력된다 -- arr은 &arr로 변경 + arr[i] 값 ≠> &arr[i] 주소
        // 하지만) arr과 &arr의 출력값은 같으므로 &&는 &로 1회만 실행됨을 짐작
        
        (그렇다면 배열의 '[]'의미는 [] == * 로 해석할 수 있다) arr[i]
        (이는 추가로 []를 소괄호로 치환을 한다면) arr[i] == *(arr+i) ==> [] = *()
        // +) 단! 2차원 배열 이상 선언 후 1차원 call 시 (int a[][];  *a  or %d, a[]) 주소값을 가진다!
        
        ∴ arr이라는 배열 변수이름은 그 자체로 &arr로 주소값을 가지지만 '[]'로 표현이 변한다!
        주소를 가르키는 'arr+i == &arr+i'과
          값을 가르키는 'arr[i] == *(arr+i) =(i가 0이라면)= *(arr)'을 완벽하게 구분하자!
          
        // & - '&' 1개는 n차원의 {} 중괄호 1개를 벗어날 수 있음
        // arr[][] = { { x, , ---}, {} --- }                             arr = &&를 가짐
        // 'arr[] = &x'가 기준! arr[]+n은 {x를 기준으로 +가 됨}            arr[] = &와 [] 상쇄 = &arr { &x , }
        // '&arr[] = &{x}'가 기준! &arr[]+n == arr+n 은 {x}를 기준으로 +   &arr[] = 앞뒤의 &, [] 상쇄 = &arr = &{ x , }
        // '&arr = & { {x} }'가 기준! &arr+n 은 { {x} }를 기준으로 +       &arr = &&&arr = &{ { x , } }
    */
    
    pointer-arr(int arr[];) - 배열포인터는 1차원은 의미가 거의 없음 => 포인터가 배열을 가르키면 자동적으로 1차원 배열형식으로 처리하기 때문!
    // 포인터의 배열이 아니기에 ()로 묶고, 가르키는 배열의 크기를 []담는다
    // 기존 포인터가 자동 1차원이기에 *ptr[]의 []에는 [0]이 된다 -- 배열의 시작은 0이기에 생략되었다고 보면 *ptr == *ptr[1]
    datatype (*var)[] = pointing var address;
    // int (*ptr_arr)[] = &arr;  +  *prt_cop = *ptr_arr == &(*ptr_arr)[0] -- (*ptr)[] == arr;
    
    // p-a(int (*var[]))는 다른 값의 주소값 1개를 가지는 포인터
    // a-p(int *var[])는 여러 개의 주소값을 가지는 포인터
    
    arr-pointer
    datatype *var[]; // 여러 개의 주소값을 가지므로 for로 초기화
    // 문자배열의 %s출력의 경우 시작주소~\n까지 출력함을 이용하여
    // char a[30][30]; int *ptr[30]; for(*ptr[i] = a[i][0])  --> %s, *ptr[i]면 문자가 출력이된다
    
    function - using var : local --> global  && (parameter) 
    void func_name(int var){}  //  use other func  -->  func_name(num);
    
    func  < - parameter & return - > func
    
    call-by-value : func(a, b) --> void func(int a, int b)
    call-by-reference : func(&a, &b)  --> void func(int *a, int *b)
              cbr-arr : func(arr)     --> void func(int *arr / int (*arr)[] )
    
    prototype : #include ~  void func(); void func();  ~ main
    
    // 재귀함수 - recursion -- stress test
    
    
    
    
    
    
    
