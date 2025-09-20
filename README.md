# SNow-CAD-notes

//Class work – looping through an array to see if they are valid emails:

var extEmails = 'uadive@gmail.com,joycemani@gmail.com, olukay@gmail.com';

var arrEmails = extEmails.split(',');

for (var i=0; i< arrEmails.length; i++){

if(isEmail(arrEmails[i]) == false){
gs.print('Invalid Email Found');
break;
}

}

function isEmail(ema){

var ismail = false;

if(ema.indexOf('@') > -1 && ema.indexOf('.com')> -1){
ismail = true;
}else{
ismail = false;
}
return ismail
}

//Example 3. 
var extEmails = '23,21, 44, 40, 99, 897';

var arrEmails = extEmails.split(',');

for (var i=0; i< arrEmails.length; i++){
var val = parseInt(arrEmails[i]);
gs.print(typeof val);
}

//Example 4
var extEmails = '23,21,44,234,456,Uday,Kishore,Gadiparthi';

var arrEmails = extEmails.split(',');

var str = [];
var num = [];

for (var i=0; i< arrEmails.length; i++){

if (i <= 4){
num.push(arrEmails[i]);
}else{
str.push(arrEmails[i]);
}

};

gs.print(str.toString());
gs.print(num.toString());

