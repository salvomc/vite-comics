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
            <div class="header-container">
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
@use '../styles/partials/variables' as *;
@use '../styles/generals' as *;

.header-container {
    max-width: 1300px;
    margin: 0 auto;
    font-size: 12px;
    .row{
            width: 100%;
            padding: 20px 0;
            display: flex;
            align-items: center;
            justify-content: space-between;

            img{
            width: 80px;
            }
        
            .col{
                    gap: 30px;
                    list-style: none;
                    display: flex;
                    text-transform: uppercase;
            
                    li{
                    
                        a:hover {
                                    border-bottom: 1px solid $main-blue-color;
                                    color: $main-blue-color;
                                }
            
                    }

                }
        }
}

</style>