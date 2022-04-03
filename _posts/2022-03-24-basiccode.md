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
      '+ '- '* /(quotient) %(remainder)
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
    Array
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
    datatype *var = pointing var address; // int *ptr = &arr;
    + **var = another pointer address;   // int **prt_a == *ptr;
    // 기본 포인터는 1차원 배열로 입출력 ∴ 2차원 이상의 접근은 배열-포인터가 필요함
    
    Array - Pointer relationship
    pointer +1(calcution) => datatype as much as change
      // int *ptr +1 => 00000000 +1 = 00000004  <-> &(*ptr) +1 => 00000000 +1 = 00000012
    int arr[]; int *ptr = &arr // arr == &arr[0] = ptr == &ptr[0] -> arr+1~
    // *ptr == arr[i] == *(arr+i) == *(ptr+i) == *(i+ptr) == ?? i[ptr]
    
    pointer-arr(int arr[];)
    datatype (*var)[] = pointing var address; // int (*ptr_arr)[] = &arr;  +  *prt_cop = *ptr_arr == &(*ptr_arr)[0]
    
    
    
    
    
    
    
    
    
