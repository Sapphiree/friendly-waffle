# friendly-waffle
just testing a JavaScript program to learn
var valor=[];
var palos = ["p", "d", "c", "t"];
var baraja = [];

 for (var i = 0; i < palos.length; i = i + 1) {
  for (var j = 1; j <= 12; j = j + 1) {
    baraja[baraja.length] = { palo: palos[ i ], valor: j };
  }
}
function barajar(baraja){
var numero_azar;

numero_azar = Math.floor(Math.random() * baraja.length);
var carta01 = baraja[ numero_azar ];
var lugar01 = numero_azar;

numero_azar = Math.floor(Math.random() * baraja.length);
var carta02 = baraja[ numero_azar ];
var lugar02 = numero_azar;

baraja[ lugar02 ] = carta01;
baraja[ lugar01 ] = carta02;
   

return baraja;
}

var croupier={};
  for (var c=0; c<100; i=i+1) {
 croupier.barajar=barajar(baraja);
  }


console.table(baraja);
