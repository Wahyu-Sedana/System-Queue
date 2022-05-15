<template>
      <div class="mt-2">
        <span class="mr-2 display-none mb-0" id="clock"></span>
        <p id="date" class="text-center headline mt-0"></p>
      </div>
</template>

<script>
export default {
    
}

window.onload = displayClock();

var monthNames = [ 'Januari', 'Februari', 'Maret', 'April', 'Mei', 'Juni', 'Juli', 'Agustus', 'September', 'Oktober', 'November', 'Desember'];
var days = ['Minggu', 'Senin', 'Selasa', 'Rabu', 'Kamis', 'jumat', 'Sabtu'];
function displayClock(){
    setInterval(() => {
      var currentdate = new Date(); 
      var date = days[currentdate.getDay()] + " "
                + currentdate.getDate() + "-"
                + monthNames[currentdate.getMonth()]  + "-" 
                + currentdate.getFullYear();
      var clock = currentdate.getHours() + ":"  
                + currentdate.getMinutes() + ":" 
                + currentdate.getSeconds();
                
      document.getElementById('clock').innerHTML = clock;
      document.getElementById('date').innerHTML = date;
    }, 1000);
}
</script>