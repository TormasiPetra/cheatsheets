anonim függvény 
    nincs neve a függvénynek

call  back függvény 
    function(response){
    console.log(response)}

DOM manipuláció 

ciklus 
    számláló segítégével 



API - azok az adatok, amiket felhasználunk, átültetjük saját felhasználásra 

    https://restcountries.com/
https://restcountries.com/v3.1/all
rickandmortyapi.com

ha új dolog van, akkor érdemes olvasni arról, hogy tudjuk értelmezni 

JSON - mint javascriptes objektumok egy tömbbe rendezvbe
    javascript object notation

fetch 
    nem azonnal indul el 
    valamikor a háttérben lefut

    ha valamit szeretnénk ezzel, akkor ezt kell bemásolni: 


    fetch('https://restcountries.com/v3.1/all')
.then(function (response){
    console.log(response.json)
} )

.then(function(responsejson/*  data */){
    console.log(responsejson/*  data */) //itt tudunk a kapott adattal dolgozni
})



async // ezen belül az await paranccsal ellátott fv-eket megvárja az utána lévő sor

await // megvárja, amig befejezi 

const demo = async () => {
  const response = await fetch("https://restcountries.com/v3.1/all")
  console.log(response)
  const data = await response.json()
  console.log(data);
}

demo()

// összeeszedjük az adatokat utána megkapjuk
const getCountries = async () => {
  const response = await fetch("https://restcountries.com/v3.1/all")
  console.log(response)
  const data = await response.json()
  return data
}

const run = async () => {
  const data = await getCountries() 
  console.log(data);
  
}

run ()