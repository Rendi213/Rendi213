<h1>contoh text-to-speech </h1>
Berikut adalah contoh sederhana untuk menggunakan Text-to-Speech (TTS) di JavaScript, yang dapat dijalankan di browser:

<pre>
&lt;!DOCTYPE html&gt;
&lt;html lang="id"&gt;
&lt;head&gt;
    &lt;meta charset="UTF-8"&gt;
    &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;
    &lt;title&gt;Text-to-Speech Example&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;/body&gt;
    &lt;h1&gt;Text-to-Speech Demo&lt;/h1&gt;
    &lt;textarea id="text-to-read" rows="5" cols="30"&gt;Halo, ini adalah contoh penggunaan text to speech di JavaScript.&lt;/textarea&gt;
    &lt;br&gt;
    &lt;button onclick="speak()"&gt;Baca Teks&lt;/button&gt;
</pre>
    <script>
        function speak() {
            const text = document.getElementById('text-to-read').value;
            const utterance = new SpeechSynthesisUtterance(text);
            speechSynthesis.speak(utterance);
        }
    </script>
</body>
</html>

➖➖➖

Penjelasan:

SpeechSynthesisUtterance digunakan untuk membuat objek yang berisi teks yang akan dibacakan.

speechSynthesis.speak() digunakan untuk memulai proses pembacaan teks.


Saat Anda membuka halaman ini di browser, Anda dapat mengetikkan teks di kotak teks dan menekan tombol "Baca Teks" untuk mendengar teks yang dibacakan oleh browser menggunakan Text-to-Speech.

