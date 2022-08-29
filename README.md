# forest-view
Sample Game for practicing game optimization (reduce draw call, object pooling, resource load)

-Atlas digunakan untuk packing asset button pada main menu. Sebelum menggunakan atlas, jumlah batches 4 dan SetPass call 2. Setelah menggunakan batches berubah menjadi 3.
-Pada audio manager, memanggil hanya resource audio yang dipakai pada gameplay scene
-static batching digunakan pada asset asset pada gameplay, sebelum dilakukan static batching, batches berkisar 3000, kemudian setelah distatic batch mejadi 600 an.
-object pooling pada mushroomspawner membuat batches stabil dikisaran 900-1000
