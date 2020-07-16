<html>
 <head> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>Most beautiful places</title> 
 <style>
   body{
  background-color:orange;
}
header{
  font-weight:bold;
  text-align: center;
  font-family:Times New Roman;
  border:2px solid black;
  font-size:200%;
  background-color:yellow;
  
}
.card{
  display:flex;
  flex-wrap:wrap;
  justify-content:space-around;
  font-size:180%;
  font-weight:bold;
  font-family:Times New Roman;
}
.details{
 border:2px solid black;
 width:400px;
 margin:20px;
 padding:10px;
 border-radius:10px;
 transition:1s;
}
.details:hover{
 width:430px;
 box-shadow:4px 4px 4px 5px black;
}
footer{
  font-weight:bold;
  text-align:center;
  border:2px solid black;
  border-radius:3px;
}
 </style>
 </head> 
 <body>
 <script>
     var places={
     india:[
       {
       Country:"India",
       State:"Uttar Pradesh",
       Place:"Tajmahal"
       },
       {
       Country:"India",
       State:"Rajasthan",
       Place:"Amber Palace"
       },
       {
       Country:"India",
       State:"Rajasthan",
       Place:"Hawamahal"
       },
       {
       Country:"India",
       State:"Andhra Pradesh",
       Place:"Araku Valley"
       }
       ],
    usa:[
       {
       Country:"USA",
       Place:"Grand Canyon National Park"
       },
       {
       Country:"USA",
       Place:"Yellow Stone National Park"
       },
       {
       Country:"USA",
       Place:"Disney land park"
       },
       {
       Country:"USA",
       Place:"Zion National Park"
       }
       ]
     
}
var body=document.body;
var header=document.createElement("header");
header.textContent="Beautiful Places";
body.append(header);
var card=document.createElement("div");
card.classList.add("card");
body.append(card);
for(i=0;i<places.india.length;i++)
{
var details=document.createElement("div");
details.classList.add("details");
card.append(details);

var country=document.createElement("p");
country.textContent="Country: "+places.india[i].Country;
details.append(country);

var state=document.createElement("p");
state.textContent="State: "+places.india[i].State;
details.append(state);

var place=document.createElement("p");
place.textContent="Place: "+places.india[i].Place;
details.append(place);


}

for(i=0;i<places.usa.length;i++)
{
var details=document.createElement("div");
details.classList.add("details");
card.append(details);

var country=document.createElement("p");
country.textContent="Country: "+places.usa[i].Country;
details.append(country);

var place=document.createElement("p");
place.textContent="Place: "+places.usa[i].Place;
details.append(place);
}
var footer=document.createElement("footer");
footer.textContent="© All rights reserved 2020";
body.append(footer);

 </script>
 </body>
</html>
