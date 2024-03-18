# SCRIPT-MINING-VERUS-HYBRID-ALL-FOR-ONE

Untuk script nya yang saya gunakan ini saya tempatkan di rc.local . Jadi nantinya ngga perlu buat crontab autorun lagi. 

Karena dengan menempatkan script ini di rc.local maka ketika reboot atau mati lampu sudah otomatis langsung jalan mining nya.

Letak dari lokasi rc.local ini berada di folder etc, lalu cari saja file dengan nama rc.local.

Untuk lebih cepatnya, bisa dengan langsung menulis scriptnya melalui perintah :

sudo nano /etc/rc.local

1. Script yang pertama ini saya gunakan kalau install ccminer nya bukan di root. Dalam kasus saya ini, saya install ccminer nya di dalam user atas nama guntur. 
-------------------------------------------------------
/home/guntur/ccminer/ccminer -a verus -o stratum+tcp://ap.luckpool.net:3956 -u RX7GExSquvgUrdac9nH4TDKnZvGjyXaFth.all-for-one -p hybrid,d=8000S,xn=60F,t=1 -t 4
exit 0

-------------------------------------------------------------
2. Script yang kedua ini digunakan kalau instalasi CCminer nya ada di dalam root.

------------------------------
/root/ccminer/ccminer -a verus -o stratum+tcp://ap.luckpool.net:3956 -u RX7GExSquvgUrdac9nH4TDKnZvGjyXaFth.all-for-one -p hybrid,d=8000S,xn=60F,t=1 -t 4
exit 0

---------------------
Nah tinggal ganti aja dengan wallet verus kalian. 
