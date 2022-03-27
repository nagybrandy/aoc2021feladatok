# Szonáris szimatolás 2.

Minden egyes mérést számba venni korántsem volt olyan jó ötlet, mint amilyennek először tűnt. Egyszerűen csak túl nagy a zaj a mért adatokban.

Ehelyett vegyük inkább az egymást követő hármasokat. Például az előző példában:

```
199  A      
200  A B    
208  A B C  
210    B C D
200  E   C D
207  E F   D
240  E F G  
269    F G H
260      G H
263        H
```

Kezdjük először azzal, hogy összehasonlítjuk az első és második "hármasmérést". Az első első hármas adatait A-val jelöltük (199, 200, 208), az ő összegük 199+200"208=607. A második hármas méréseit B-vel jelölik, ezek összege 618. A második hármas méréseinek összege nagyobb, mint az első hármas méréseinek az összege, tehát az első összehasonlítás növekedés mutatott.

Most az lesz a feladatod, hogy megszámold, hogy hány hármasmérés mutat növekedést. Tehát hasonlítsd össze A-t B-vel, aztán B-t C-vel, majd C-t D-vel és így tovább. Akkor hagyd abba, amikor már nem lehet több hármasmérést formálni a rendelkezésre álló mérésekből.

A fenti példában a hármasmérések összegei a következőképpen alakulnak:

```
A: 607 (Nincs előző összeg)
B: 618 (nőtt)
C: 618 (nem változott)
D: 617 (csökkent)
E: 647 (nőtt)
F: 716 (nőtt)
G: 769 (nőtt)
H: 792 (nőtt)
```

Ebben a példában 5 összeg van, ami nagyobb mint az előző összeg.

**Az adatokban a hármasmérések összegével számolva hány hármasmérés mutat növekedést?**
