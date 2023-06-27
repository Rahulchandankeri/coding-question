
#1 Captialize First Letter In A Sentence

// RESULT
const str = "wef e   ewfwe this is saMple teXt";
 
 // METHOD 1
const opStr = str.split(" ").map((txt, i) =>  (txt.slice(0,1).toUpperCase() + txt.slice(1).toLowerCase())).join(" ") ;
console.log(opStr);


// METHOD 2
let opStr2 = ""
for(let i = 0; i < str.length - 1; i++) {
    if(i == 0) {
           opStr2+=str[i].toUpperCase();
    }
    if(str.charCodeAt(i) == 32 ){
        opStr2+=str[i+1].toUpperCase();
    } else{
      opStr2+=str[i+1].toLowerCase()
    }
}
console.log(opStr2)

