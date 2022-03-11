<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="vendor/tailwind.css">
</head>
<body class="duration-1000 min-h-screen flex items-center justify-center bg-cover bg-center">
    
    <div id="box" class="w-96 h-96 bg-white shadow-xl flex items-center justify-center text-3xl">

    </div>
    

    <script>

        var images = [
            'https://pixabay.com/get/g40154c0097ba87d7a33837b692c7fa28cff933adc8aeedba9c9f52a898fb917abb4340790d283e65355a8e2ac6a88a40e24918a8beb802054f1d64cf9c43ec39_640.jpg',
            'https://pixabay.com/get/g1119470324604872f669f99e034a7fe176a94e7ecfbde2159c0281c31572d0040c6176274298200738449d4dc165c393ecf8f98df4a9d4373797a9a9ed7c07bc_640.jpg',
            'https://pixabay.com/get/g652e5fed66fe9b527f62960a36f92c015ad852f643b7e8fd24156c1d61af7128ea5979168956e05ef1bb396b172fd6f0fa41eeb7306c370f5a6f2032ddd66ae6_640.jpg',
            'https://pixabay.com/get/g9702f01a0d38f215330d2e05d41ef7d4015d2976a8ff62a87d4960111b7c354e44cc4820e067aa8b7215f9cf9c7dfc19403ea31b7fe770819bfde04b9dc6deff_640.jpg',
            'https://pixabay.com/get/g9981716449ad93c1b983b86005c9b0d9813cdaa6b0d1679cfaa7ad9e02821bd388bbc195f53a483dc440e6c30542853bf7293422fbf2d4926531c3c6cfd869e0_640.jpg',
            'https://pixabay.com/get/g2846a5ae42962f3e716626f3a887bd1784e5edfa7202208c4f8511251f47dd550bfe65c5c1248da10f9de109fdcdb3b8186f9a815b67551f38455575e6706211_640.jpg'
        ];

        var colori = [
            'red', 'blue', 'pink', 'green', 'beige', '#0f0'
        ];

        var parole = [
            'fermo', 'ancora', 'resto', 'qua', '...'
        ]

        var i = 0;
        var ii = 0;
        var iii = 0;

        function cambiaParole() {
            document.querySelector("#box").innerHTML = parole[ii];
            if (ii < 5) {
                ii = ii + 1; 
            
            } else {
                ii = 0;
            }
        }

        function cambiaColore() {

            document.body.style.backgroundColor = colori[i];
            if (i < 5) {
                i = i + 1; 
            
            } else {
                i = 0;
            }
        }

            console.log(i, colori[i]);

        document.body.style.backgroundBlendMode = 'color-burn'  
        document.body.style.backgroundImage = 'url('+images[0]+')';
        

        function cambiaImmagine() {
        document.body.style.backgroundImage = 'url('+images[iii]+')';
        if (iii < 5) {
        iii = iii + 1;
        } else {
            iii = 0;
        }

    }

        setInterval(cambiaColore, 1000);
        setInterval(cambiaParole, 1000);
        setInterval(cambiaImmagine, 1000);

        

        console.log(images[2]);
       


    </script>


</body>
</html>
