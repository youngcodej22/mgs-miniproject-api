// https://json-generator.com/#

[
'{{repeat(30)}}',
{
\_id: '{{objectId()}}',
index: '{{index()}}',
date: '{{date(new Date(2022, 0, 1), new Date(), "YYYY-MM-dd")}}',
money: function (tags){
var myArray = ['in', 'out'];
var rand = Math.random()*myArray.length | 0;
var result = myArray[rand];
return result;
},
type: function (tags){
var myArray = ['mart', 'restaurant', 'personal', 'cafe'];
var rand = Math.random()*myArray.length | 0;
var result = myArray[rand];
return result;
},
item: '',
price: ''
}
]
