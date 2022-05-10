# Simple-Calculator(sol)

// SPDX-License-Identifier: GPL-3.0

//上面第一行不是註解，是授權開放(GPL-3.0)或不開放(UNLICENSED)

pragma solidity >=0.7.0 <0.9.0;

contract calculate{    //合約簡易加減計算機
    int private a ;    //結果儲存

    function add(int x, int y) public returns(int z){    //加法
      a = x + y;
      z = a;
    }
     
    function sub(int x, int y) public returns(int z){   //減法
      a = x - y;
      z = a;
    }
    
    function total() public view returns(int){          //回傳結果 
        return a;
    }
}
