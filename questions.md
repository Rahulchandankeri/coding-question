
#1 Capitalize First Letter In A Sentence


 <code>
// INPUT STRING
  const str = "wef e   ewfwe this is saMple teXt";
 </code>
 
 // METHOD 1
 <code>
const opStr = str.split(" ").map((txt, i) =>  (txt.slice(0,1).toUpperCase() + txt.slice(1).toLowerCase())).join(" ") ;
console.log(opStr);
</code>

// METHOD 2
<code>
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
</code>

