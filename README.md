## Solidity-DataTypes-Lib.  
It contains all solidity data types    
```
// SPDX-License-Identifier: MIT
pragma solidity >=0.8.0;
import "./Types.sol";
contract Example{
    struct Data{
       uint256 attributeA;
       bytes attributeB;
    }
    function getType()public pure returns(Types.Type[] memory){
        Types.Type[] memory dataType=new Types.Type[](2);
        dataType[0]=Types.Type.UINT256;
        dataType[1]=Types.Type.BYTES;
        return dataType;
    }
}
```