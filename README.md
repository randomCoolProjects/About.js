# About.js

Obtenha todas informações disponíveis, tais como Nível de Bateria, navegador, sistema operacional, localização &amp; mais.  

# Download ou importação  
Você pode baixar o arquivo JS <a href="https://randomcoolprojects.github.io/About.js/about.js" downlaod="about.js">aqui</a>.  
Ou, você pode importar diretamente do servidor:  
```html
<script src="https://randomcoolprojects.github.io/About.js/about.js"></script>
```
# Usando
É simples e fácil de usar, siga o código abaixo como exemplo:
```javascript
var about = About();
window.setTimeout(function(){
  console.log(about);
  var sistema = about.Device.OperatingSystem;
  var cidade = about.Location.City; // O rastreamento é feito via IP
  console.log('Você mora em ' + cidade);
  console.log('Seu sistema operacional é ' + sistema);
}, 2000); // 2 segundos de tempo para receber os dados
```
* __É nescessário esperar um curto período de tempo para as informações chegarem. 2 segundos perece bom.__
# Demo
Você pode ver uma demonstração <a href="https://randomcoolprojects.github.io/About.js/index.html">aqui</a>
# Serviços externos
Usamos os seguintes serviços externos:  
<a href="http://ipinfo.io">http://ipinfo.io</a> para obter o endereço de ip;  
<a href="https://ipapi.co/json/">https://ipapi.co/json/</a> para rastrear o ip;  
