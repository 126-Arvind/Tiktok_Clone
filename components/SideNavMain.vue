<template>
   
    <div 
    id="SideNavMain" 
    :class="route.fullPath === '/' ? 'lg:w-[310px]' : 'lg:w-[220px]'" 
    class="fixed z-20 bg-white pt-[70px] h-full lg:border-r-0 border-r w-[75px] overflow-auto"
>
<div class="lg:w-full w-[55px] mx-auto">
    <NuxtLink to="/">
        <MenuItem iconString="For You" colorString="#F02C56" sizeString="30"/>
    </NuxtLink>
    <MenuItem iconString="Following" colorString="#000000" sizeString="27"/>
    <MenuItem iconString="LIVE" colorString="#000000" sizeString="27"/>


<div class="border-b lg:ml-2 mt-2" />
<div class="lg:block hidden text-xs text-gray-600 font-semibold pt-4 pb-2 px-2">
    Suggested accounts
</div>
<div class="lg:hidden block pt-3"/>
<div class="cursor-pointer">
    <MenuItemFollow />
</div>
<button class="lg:block hidden text-[#FO2C56] pt-1.5 pl-2 text-[13px]">sell all</button>



    </div>
    
</div>

    </template>
    
    <script setup>
   const route = useRoute();
    
    </script>