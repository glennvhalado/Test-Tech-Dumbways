# test-tech-dumbways

## Soal No. 3

![nomor3](https://user-images.githubusercontent.com/34154595/127832320-631dfcc4-f1c5-46e3-bb85-8ee75816f32d.png)

> - Bahasa yang digunakan adalah Javascript
> - Menggunakan compiler https://es6console.com/krudele0/

```

var s = '';
var pola = 5;

function pascal(n) {
    var a = 1;
    var i = 1;

    while(i <= n) {
        a *= i;
        i++;
    }

    return a;
} 

for (var i=0; i < pola; i++) {

    for(var j = pola; j >= i; j--) {
        s += ' ';
    }

    for(var j = 0; j <= i; j++) {
        s += pascal(i) / ( pascal(j) * pascal (i - j)) + ' ';
    }

    s += '\n';
}

console.log(s);

```
