# MinArray.sol
MinArray.sol
pragma solidity ^0.8.20;
contract MinArray {
    function min(uint[] memory arr) public pure returns(uint) {
        uint m = arr[0];
        for(uint i=1;i<arr.length;i++){
            if(arr[i] < m) m = arr[i];
        }
        return m;
    }
}
