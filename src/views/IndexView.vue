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
                    <a href="#" class="text-lg text-red-300 hover:opacity-50">Cakes</a>
                    <a href="#" class="text-lg text-red-300 hover:opacity-50">Cupcakes</a>
                    <a href="#" class="text-lg text-red-300 hover:opacity-50">Cookies</a>
                    <a href="#" class="text-lg text-red-300 hover:opacity-50">Brownies</a>
                    <a href="#" class="text-lg text-red-300 hover:opacity-50">Breads</a>
                    <a href="#" class="text-lg text-red-300 hover:opacity-50">Drinks</a>
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
                    <a href="#" class="text-lg bg-red-200 lg:p-10 p-8 flex lg:w-full w-32 justify-center items-center hover:opacity-50">Cakes</a>
                    <a href="#" class="text-lg bg-red-100 lg:p-10 p-8 flex lg:w-full w-32 justify-center items-center hover:opacity-50">Cupcakes</a>
                    <a href="#" class="text-lg bg-red-200 lg:p-10 p-8 flex lg:w-full w-32 justify-center items-center hover:opacity-50">Cookies</a>
                    <a href="#" class="text-lg bg-red-100 lg:p-10 p-8 flex lg:w-full w-32 justify-center items-center hover:opacity-50">Brownies</a>
                    <a href="#" class="text-lg bg-red-200 lg:p-10 p-8 flex lg:w-full w-32 justify-center items-center hover:opacity-50">Breads</a>
                    <a href="#" class="text-lg bg-red-100 lg:p-10 p-8 flex lg:w-full w-32 justify-center items-center hover:opacity-50">Drinks</a>
                </div>
            </div>
        </section>
        <section class="mx-24 lg:mx-6 py-8 lg:px-20">
            <div class="text-2xl mb-10">Cakes</div>
            <div class="grid grid-cols-2 lg:grid-cols-5 gap-4 justify-between pb-11">
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cakes/cake1.jpg" alt="cake 1" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Birthday Cake
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cakes/cake2.jpg" alt="cake 2" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Birthday Cake
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cakes/cake3.jpg" alt="cake 3" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Birthday Cake
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cakes/cake4.jpg" alt="cake 4" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Birthday Cake
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto hidden lg:block">
                    <img src="../assets/cakes/cake5.jpg" alt="cake 5" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Birthday Cake
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
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
        <section class="mx-24 lg:mx-6 py-8 lg:px-20">
            <div class="text-2xl mb-10">Cupcakes</div>
            <div class="grid grid-cols-2 lg:grid-cols-5 gap-4 justify-between pb-11">
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cupcakes/cupcake1.jpg" alt="Cupcake 1" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cupcakes
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cupcakes/cupcake2.jpg" alt="Cupcake 2" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cupcakes
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cupcakes/cupcake3.jpg" alt="Cupcake 3" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cupcakes
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cupcakes/cupcake4.jpg" alt="Cupcake 4" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cupcakes
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto hidden lg:block">
                    <img src="../assets/cupcakes/cupcake5.jpg" alt="Cupcake 5" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cupcakes
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
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
        <section class="mx-24 lg:mx-6 py-8 lg:px-20">
            <div class="text-2xl mb-10">Cookies</div>
            <div class="grid grid-cols-2 lg:grid-cols-5 gap-4 justify-between pb-11">
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cookies/cookie1.jpg" alt="Cookie 1" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cookies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 30.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cookies/cookie2.jpg" alt="Cookie 2" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cookies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 30.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cookies/cookie3.jpg" alt="Cookie 3" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cookies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 30.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/cookies/cookie4.jpg" alt="Cookie 4" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cookies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 30.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto hidden lg:block">
                    <img src="../assets/cookies/cookie5.jpg" alt="Cookie 5" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Cookies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 30.000
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
        <section class="mx-24 lg:mx-6 py-8 lg:px-20">
            <div class="text-2xl mb-10">Brownies</div>
            <div class="grid grid-cols-2 lg:grid-cols-5 gap-4 justify-between pb-11">
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/brownies/brownie1.jpg" alt="Brownie 1" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Brownies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/brownies/brownie2.jpg" alt="Brownie 2" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Brownies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/brownies/brownie3.jpg" alt="Brownie 3" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Brownies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/brownies/brownie4.jpg" alt="Brownie 4" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Brownies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto hidden lg:block">
                    <img src="../assets/brownies/brownie5.jpg" alt="Brownie 5" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Brownies
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
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
        <section class="mx-24 lg:mx-6 py-8 lg:px-20">
            <div class="text-2xl mb-10">Bread</div>
            <div class="grid grid-cols-2 lg:grid-cols-5 gap-4 justify-between pb-11">
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/bread/bread1.jpg" alt="Bread 1" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Bread
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/bread/bread2.jpg" alt="Bread 2" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Bread
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/bread/bread3.jpg" alt="Bread 3" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Bread
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/bread/bread4.jpg" alt="Bread 4" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Bread
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto hidden lg:block">
                    <img src="../assets/bread/bread5.jpg" alt="Bread 5" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Bread
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 50.000
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
        <section class="mx-24 lg:mx-6 py-8 lg:px-20">
            <div class="text-2xl mb-10">Drinks</div>
            <div class="grid grid-cols-2 lg:grid-cols-5 gap-4 justify-between pb-11">
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/drinks/drink1.jpg" alt="Drink 1" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Drinks
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 20.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/drinks/drink2.jpg" alt="Drink 2" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Drinks
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 20.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/drinks/drink3.jpg" alt="Drink 3" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Drinks
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 20.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto">
                    <img src="../assets/drinks/drink4.jpg" alt="Drink 4" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Drinks
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 20.000
                            <div class="bg-red-300 w-8 h-8 flex items-center justify-center rounded-full cursor-pointer hover:opacity-50">
                                <i class="bi bi-cart-plus text-lg text-white"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer max-w-xs mx-auto hidden lg:block">
                    <img src="../assets/drinks/drink5.jpg" alt="Drink 5" class="w-full h-auto object-cover">
                    <div class="bg-red-100 w-full p-4">
                        <div class="mb-1">
                            Drinks
                        </div>
                        <div class="flex items-center mb-1 space-x-1">
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                            <i class="bi bi-star-fill text-yellow-400"></i>
                        </div>
                        <div class="flex items-center justify-between">
                            Rp 20.000
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
                        <p class="text-lg">Cakes</p>
                        <p class="text-lg">Cupcakes</p>
                        <p class="text-lg">Cookies</p>
                        <p class="text-lg">Brownies</p>
                        <p class="text-lg">Bread</p>
                        <p class="text-lg">Drinks</p>
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