<!doctype html>
<title>Site Maintenance</title>
<style>
  body { text-align: center; padding: 150px; }
  h1 { font-size: 50px; }
  body { font: 20px Helvetica, sans-serif; color: #333; }
  .container { display: block; text-align: left; width: 650px; margin: 0 auto; }
</style>
<div class='container'> 
    <img src="./umn.png" alt="Logo" width="100" height="200">
    <div id="countdown"></div>
    <script>
        function updateCountdown() {
            const targetTime = new Date('2023-07-17T20:00:00'); // Ganti dengan waktu target kapan situs akan kembali online (format: 'YYYY-MM-DDTHH:mm:ss')
            const now = new Date();
            const timeLeft = targetTime - now;
    
            if (timeLeft <= 0) {
                document.getElementById('countdown').innerHTML = 'Situs telah kembali online!'; // Pesan setelah waktu target tercapai
            } else {
                const days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
                const hours = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((timeLeft % (1000 * 60)) / 1000);
                
                document.getElementById('countdown').innerHTML = `The site will be back online in: ${days} hari, ${hours} jam, ${minutes} menit, ${seconds} detik`;
            }
        }
    
        // Panggil fungsi updateCountdown setiap detik
        setInterval(updateCountdown, 1000);
    </script>
    

    <h1>We&rsquo;ll be back soon!</h1>
    
        <p>Sorry for the inconvenience but we&rsquo;re performing some maintenance at the moment.
        If the probelem still persists contact us helpdesk.umn.ac.id</a>
        , otherwise repairs are in progress and we&rsquo;ll be back online shortly!</p>
        <p>&mdash; TEAM IT</p>
    
</div>
