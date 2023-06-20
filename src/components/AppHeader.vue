<script>
export default {
    data() {
        return {
            arrayListHeader:
            [
                {label: 'CHARACTERS', link:'#', active: false},
                {label: 'COMICS', link:'#', active: false},
                {label: 'MOVIES', link:'#', active: false},
                {label: 'TV', link:'#', active: false},
                {label: 'GAMES', link:'#', active: false},
                {label: 'COLLECTIBLES', link:'#', active: false},
                {label: 'VIDEOS', link:'#', active: false},
                {label: 'FANS', link:'#', active: false},
                {label: 'NEWS', link:'#', active: false},
                {label: 'SHOP', link:'#', active: false},
            ]
            
        }
    }
}
</script>

<template>
    
    <div>
        <header>
            <div class="container">
                <div class="row">
                    <img class="col" src="/img/dc-logo.png" alt="">
                    <ul class="col">
                        <li v-for="(link, index) in arrayListHeader" :key="index"> 
                            <a :href="link.link"> {{ link.label }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </header>
    </div>

</template>

<style lang="scss" scoped>
@use '../partials/variables' as *;
@use '../partials/generals' as *;
.row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px 0;
    width: 100%;

    img {
        width: 80px;
    }
    
    .col{
        display: flex;
        gap: 30px;
        text-transform: uppercase;
        list-style: none;
        
            li{
                
            a:hover {
                color: $blue;
                border-bottom: 1px solid $blue;
                }
        
            }

        }
    }

</style>