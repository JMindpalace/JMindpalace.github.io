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
    Value Calcution - unsigned(- -> all +)
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
