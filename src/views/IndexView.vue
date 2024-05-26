<template>
    <div class="relative">
        <div class="relative w-full py-2 bg-red-300 text-center text-white text-xs"> Dapatkan diskon 50% Sekarang </div>
        <div class="bg-white w-full sticky top-0 z-20 shadow">
            <div class="w-full lg:px-20 px-8 flex justify-between items-center">
                <a href="#" class="flex items-center">
                    <img src="../assets/logo2.png" alt="Logo Sweetsy Bakery" class="w-20">
                    <div class="text-xl text-semi-bold text-red-300 uppercase">Sweetsy Bakery</div>
                </a>
                <div class="gap-7 items-center justify-center text-sm lg:flex hidden">
                    <a v-for="category in categories" href="#" class="text-lg text-red-300 hover:opacity-50">{{ category.name }}</a>
                </div>
                <div class="flex gap-10">
                    <a href="#" class="hover:opacity-50">
                        <i class="bi bi-search-heart-fill text-xl text-red-300"></i>
                    </a>
                    <a href="#" class="hover:opacity-50">
                        <i class="bi bi-cart-fill text-xl text-red-300"></i>
                    </a>
                </div>
            </div>
        </div>
        <section class="relative">
            <img src="../assets/background2.jpg" alt="background" class="w-screen lg:h-auto object-fill">
            <div class="absolute w-full h-full top-0 left-0 flex flex-col items-center justify-center px-96">
                <div class="text-xl lg:text-4xl tracking-wide leading-snug text-center">
                    <span class="font-bold">Dipanggang</span>
                    dengan Cinta
                    <br> 
                    <span class="font-bold">Disajikan</span> 
                    dengan Sukacita
                </div>
                <div class="cursor-pointer bg-red-400 lg:p-2 p-1 w-52 text-center text-white font-bold rounded-full text-lg lg:mt-8 mt-4 hover:opacity-50"> 
                    Beli Sekarang
                </div>
            </div>
        </section>
        <section class="bg-red-50 lg:py-20">
            <div class="text-2xl text-center py-10">
                Keuntungan yang Kami Berikan
            </div>
            <div class="w-full grid grid-cols-2 lg:flex gap-6 lg:gap-1 justify-between px-20 pb-11">
                <div class="bg-red-400 w-64 text-center text-white rounded text-lg px-5 py-5"><i class="bi bi-trophy-fill text-4xl"></i><br>Produk Berkualitas Tinggi</div>
                <div class="bg-red-400 w-64 text-center text-white rounded text-lg px-5 py-5"><i class="bi bi-cake2 text-4xl"></i><br>Varian yang Beragam</div>
                <div class="bg-red-400 w-64 text-center text-white rounded text-lg px-5 py-5"><i class="bi bi-person-heart text-4xl"></i><br>Pelanggan Puas</div>
                <div class="bg-red-400 w-64 text-center text-white rounded text-lg px-5 py-5"><i class="bi bi-truck text-4xl"></i><br>Kirim Sampai Rumah</div>
            </div>
        </section>
        <section class="mx-24 my-20">
            <div class="text-2xl mb-10">Kategori Produk</div>
            <div class="w-[362px] md:w-full overflow-x-auto">
                <div class="flex min-w-max">
                    <a v-for="(category, index) in categories" :key="index"  href="#" :class="getBackgroundClass(index)" class="text-lg bg-red-200 lg:p-10 p-8 flex lg:w-full w-32 justify-center items-center hover:opacity-50">{{ category.name }}</a>
                </div>
            </div>
        </section>
        <section v-for="(category, catIndex) in categories" :key="catIndex" class="mx-24 lg:mx-6 py-8 lg:px-20">
            <div class="text-2xl mb-10">{{ category.name }}</div>
            <div class="grid grid-cols-2 lg:grid-cols-5 gap-4 justify-between pb-11">
                <div v-for="(product, prodIndex) in category.products" :key="prodIndex" class="cursor-pointer max-w-xs mx-auto" :class="{'hidden lg:block': prodIndex === 4}">
                    <img :src="product.image" :alt="product.name" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">{{ product.name }}</div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i v-for="i in 5" :key="i" class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            {{ product.price }}
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="text-center hover:opacity-50">
                <a href="#">Lihat Semuanya</a>
            </div>
        </section>
        <section class="mx-24 my-20">
            <div class="text-xl font-bold mb-6">Sweetsy Bakery - Bakery Online se-Indonesia</div>
            <div class="text-lg">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corporis, quisquam magnam fugiat quidem quasi excepturi quam alias quos nihil soluta, eos ab consequatur atque quia reiciendis ut adipisci, suscipit itaque?</div>
        </section>
        <section class="bg-red-50">
            <div class="text-2xl text-center py-10">
                Testimoni Pelanggan
            </div>
            <div class="grid grid-rows-1 grid-flow-col gap-4 justify-center px-10 pb-11">
                <div class="bg-red-400 w-full text-center text-white rounded text-lg px-5 py-5">
                    <div>
                        <i class="bi bi-person-circle text-4xl text-red-50"></i>
                    </div>
                    <div class="font-bold">
                        syipaaln
                    </div>
                    <div>
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                    </div>
                </div>
                <div class="bg-red-400 w-full text-center text-white rounded text-lg px-5 py-5">
                    <div>
                        <i class="bi bi-person-circle text-4xl text-red-50"></i>
                    </div>
                    <div class="font-bold">
                        syipaaln
                    </div>
                    <div>
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                    </div>
                </div>
            </div>
        </section>
        <section class="bg-yellow-100 px-20 py-10">
            <div class="text-xl">Metode Pembayaran</div>
            <div class="grid grid-rows-1 grid-flow-col gap-4 justify-start my-10">
                <div class="bg-white px-10 py-10 rounded">
                    <img src="../assets/dana.png" alt="Dana" class="w-20">
                </div>
                <div class="bg-white px-10 py-10 rounded">
                    <img src="../assets/bca1.png" alt="BCA" class="w-20">
                </div>
            </div>
        </section>
        <section class="bg-yellow-100 px-20 py-10">
            <div class="text-xl mb-10">Pertanyaan Umum (FAQ)</div>
            <div class="flex flex-col gap-4">
                <div class="bg-white cursor-pointer p-4 flex flex-col gap-2">
                    <div class="flex w-full justify-between items-center">
                        <div class="font-semibold">lorem ipsum dolor sit amet consectetur adipisicing elit?</div>
                        <div><i class="bi bi-chevron-down"></i></div>
                    </div>
                </div>
                <div class="bg-white cursor-pointer p-4 flex flex-col gap-2">
                    <div class="flex w-full justify-between items-center">
                        <div class="font-semibold">lorem ipsum dolor sit amet consectetur adipisicing elit?</div>
                        <div><i class="bi bi-chevron-down"></i></div>
                    </div>
                </div>
                <div class="bg-white cursor-pointer p-4 flex flex-col gap-2">
                    <div class="flex w-full justify-between items-center">
                        <div class="font-semibold">lorem ipsum dolor sit amet consectetur adipisicing elit?</div>
                        <div><i class="bi bi-chevron-down"></i></div>
                    </div>
                </div>
                <div class="bg-white cursor-pointer p-4 flex flex-col gap-2">
                    <div class="flex w-full justify-between items-center">
                        <div class="font-semibold">Lorem ipsum dolor sit amet consectetur adipisicing elit?</div>
                        <div><i class="bi bi-chevron-down"></i></div>
                    </div>
                </div>
            </div>
        </section>
        <section class="mx-20 my-20">
            <div class="flex justify-between">
                <div class="text-2xl">Lebih Mudah Mengirim Kue untuk Orang Tersayang</div>
                <div class="bg-red-400 text-white px-5 lg:px-16 py-2 lg:py-3 rounded cursor-pointer hover:opacity-50">Beli Sekarang</div>
            </div>
        </section>
        <footer>
            <div class="bg-red-400 py-10 px-20">
                <div class="">
                    <div class="flex items-center text-2xl font-bold uppercase text-white" href="#">
                        <img src="../assets/logo3.png" alt="logo" class="w-12">
                        Sweetsy Bakery
                    </div>
                </div>
                <div class="grid grid-rows-1 grid-flow-col gap-4 justify-between text-white my-10">
                    <div>
                        <p class="text-xl text-semibold mb-5">Alamat</p>
                        <p class="text-lg">Cianjur, Jawa Barat</p>
                    </div>
                    <div>
                        <p class="text-xl text-semibold mb-5">Kategori Produk</p>
                        <p v-for="category in categories"  class="text-lg">{{ category.name }}</p>
                    </div>
                    <div>
                        <p class="text-xl text-semibold mb-5">Kontak Kami</p>
                        <p class="text-lg">+62 800 000 000</p>
                        <p class="text-lg">admin@sweetsybakery.com</p>
                    </div>
                </div>
                <div class="w-full text-center text-white text-xs"> © 2024 SWEETSY BAKERY All rights reserved </div>
            </div>
        </footer>
    </div>
</template>

<script setup>
    import { ref, reactive } from 'vue';
    
    import cake1 from '../assets/cakes/cake1.jpg';
    import cake2 from '../assets/cakes/cake2.jpg';
    import cake3 from '../assets/cakes/cake3.jpg';
    import cake4 from '../assets/cakes/cake4.jpg';
    import cake5 from '../assets/cakes/cake5.jpg';

    import cupcake1 from '../assets/cupcakes/cupcake1.jpg';
    import cupcake2 from '../assets/cupcakes/cupcake2.jpg';
    import cupcake3 from '../assets/cupcakes/cupcake3.jpg';
    import cupcake4 from '../assets/cupcakes/cupcake4.jpg';
    import cupcake5 from '../assets/cupcakes/cupcake5.jpg';

    import cookie1 from '../assets/cookies/cookie1.jpg';
    import cookie2 from '../assets/cookies/cookie2.jpg';
    import cookie3 from '../assets/cookies/cookie3.jpg';
    import cookie4 from '../assets/cookies/cookie4.jpg';
    import cookie5 from '../assets/cookies/cookie5.jpg';

    import brownie1 from '../assets/brownies/brownie1.jpg';
    import brownie2 from '../assets/brownies/brownie2.jpg';
    import brownie3 from '../assets/brownies/brownie3.jpg';
    import brownie4 from '../assets/brownies/brownie4.jpg';
    import brownie5 from '../assets/brownies/brownie5.jpg';

    import bread1 from '../assets/breads/bread1.jpg';
    import bread2 from '../assets/breads/bread2.jpg';
    import bread3 from '../assets/breads/bread3.jpg';
    import bread4 from '../assets/breads/bread4.jpg';
    import bread5 from '../assets/breads/bread5.jpg';

    import drink1 from '../assets/drinks/drink1.jpg';
    import drink2 from '../assets/drinks/drink2.jpg';
    import drink3 from '../assets/drinks/drink3.jpg';
    import drink4 from '../assets/drinks/drink4.jpg';
    import drink5 from '../assets/drinks/drink5.jpg';

    const categories = reactive([
        {
            name: 'Cakes',
            products: [
                { name: 'Birthday Cake', price: 'Rp 50.000', image: cake1 },
                { name: 'Birthday Cake', price: 'Rp 50.000', image: cake2 },
                { name: 'Birthday Cake', price: 'Rp 50.000', image: cake3 },
                { name: 'Birthday Cake', price: 'Rp 50.000', image: cake4 },
                { name: 'Birthday Cake', price: 'Rp 50.000', image: cake5 }
            ]
        },
        {
            name: 'Cupcakes',
            products: [
                { name: 'Cupcake', price: 'Rp 50.000', image: cupcake1 },
                { name: 'Cupcake', price: 'Rp 50.000', image: cupcake2 },
                { name: 'Cupcake', price: 'Rp 50.000', image: cupcake3 },
                { name: 'Cupcake', price: 'Rp 50.000', image: cupcake4 },
                { name: 'Cupcake', price: 'Rp 50.000', image: cupcake5 }
            ]
        },
        {
            name: 'Cookies',
            products: [
                { name: 'Cookies', price: 'Rp 30.000', image: cookie1 },
                { name: 'Cookies', price: 'Rp 30.000', image: cookie2 },
                { name: 'Cookies', price: 'Rp 30.000', image: cookie3 },
                { name: 'Cookies', price: 'Rp 30.000', image: cookie4 },
                { name: 'Cookies', price: 'Rp 30.000', image: cookie5 }
            ]
        },
        {
            name: 'Brownies',
            products: [
                { name: 'Brownies', price: 'Rp 50.000', image: brownie1 },
                { name: 'Brownies', price: 'Rp 50.000', image: brownie2 },
                { name: 'Brownies', price: 'Rp 50.000', image: brownie3 },
                { name: 'Brownies', price: 'Rp 50.000', image: brownie4 },
                { name: 'Brownies', price: 'Rp 50.000', image: brownie5 }
            ]
        },
        {
            name: 'Breads',
            products: [
                { name: 'Bread', price: 'Rp 50.000', image: bread1 },
                { name: 'Bread', price: 'Rp 50.000', image: bread2 },
                { name: 'Bread', price: 'Rp 50.000', image: bread3 },
                { name: 'Bread', price: 'Rp 50.000', image: bread4 },
                { name: 'Bread', price: 'Rp 50.000', image: bread5 }
            ]
        },
        {
            name: 'Drinks',
            products: [
                { name: 'Drink', price: 'Rp 20.000', image: drink1 },
                { name: 'Drink', price: 'Rp 20.000', image: drink2 },
                { name: 'Drink', price: 'Rp 20.000', image: drink3 },
                { name: 'Drink', price: 'Rp 20.000', image: drink4 },
                { name: 'Drink', price: 'Rp 20.000', image: drink5 }
            ]
        }
    ]);

    function getBackgroundClass(index) {
        return index % 2 === 0 ? 'bg-red-300' : 'bg-red-200';
    }
</script>