# LandRecord
Day 3 Assignment
pragma solidity ^0.4.17 < 0.6.12; 

contract LandRecord{
    
    string public owner;
    uint public   value ;
    string public location;
    string public area;
    string public legalId;
    
    function LandRecord(string newOwner, uint newValue, string newLocation, string newArea, string newLegalId) public{
        
        owner = newOwner;
        value = newValue;
        location = newLocation;
        area = newArea;
        legalId = newLegalId;
        
    }
    
    function setLandNewDetails(string newOwner, uint newValue) public{
        
        owner = newOwner;
        value = newValue;
        
    }
    
    function getLandCurrentDetails() public view returns(string,uint,string,string,string){
        return(owner, value, location, area, legalId);
    }
    
    
}

The test deployment of Smart contract for Land Record can be found at 0x5e177a9483e3d157ee3880dcd1316f3ac8da31d9 in
https://ropsten.etherscan.io/tx/0x15b89abc6a451a0d1c46a0fc6bb5d5cd824596d807455a2c1d0e3be37246fb9d
