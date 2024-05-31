// create a variable to hold your NFT's
const NFTs = []

// this function will take in some values as parameters, create an
// NFT object using the parameters passed to it for its metadata, 
// and store it in the variable above.
function mintNFT (_name, _eyeColor, _shirtType, _bling) {
    const NFT = {
        "name": _name,
        "eyeColor": _eyeColor,
        "shirtType": _shirtType,
        "bling": _bling
    }
    NFTs.push(NFT);
    console.log("Minted: " + _name, _eyeColor )
    
}
 
// create a "loop" that will go through an "array" of NFT's
// and print their metadata with console.log()
function listNFTs () {
 for(let i = 0; i < NFTs.length; i++) {
    console.log("\nID: \t\t" + (i + 1));
    console.log("\nName: \t\t" + NFTs[i].name);
    console.log("Eyecolor: \t" + NFTs[i].eyeColor);
    console.log("Shirt Type: " + NFTs[i].shirtType);
    console.log("Bling: \t\t" + NFTs[i].bling);
 }
}

// print the total number of NFTs we have minted to the console
function getTotalSupply() {
 console.log(NFTs.length);
}

// call your functions below this line
mintNFT("Quinn", "Black", "Polo Shirt", "Diamond");
mintNFT("Prince", "Black", "Flannel", "Diamond");
mintNFT("Kyle", "Black", "Henly Shirt", "Diamond");
mintNFT("Enzo", "Black", "Jean Jacket", "Diamond");
listNFTs();
getTotalSupply();
