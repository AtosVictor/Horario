<html>
<body>
    <div id="clock" style="font-size: 24px; font-family: Arial;"></div>
    <script>
        function updateClock() {
            const now = new Date();
            const formattedTime = now.toLocaleString('pt-BR', {
                timeZone: 'America/Sao_Paulo',
                hour: '2-digit',
                minute: '2-digit',
                second: '2-digit',
                day: '2-digit',
                month: '2-digit',
                year: 'numeric'
            });
            document.getElementById('clock').innerText = formattedTime;
        }
        setInterval(updateClock, 1000);
        updateClock();
    </script>
</body>
</html>
