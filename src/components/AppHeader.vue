<template>
    <header>
        <div class="nav-bar">
            <button @click="show"><span class="material-symbols-sharp">menu</span></button>
            <div class="dashboard">
                <h1>DashBoard</h1>
            </div>
            <div class="search-box">
                <input type="search" placeholder="Search...">
                <button>
                    <span class="material-symbols-sharp">search</span>
                </button>
            </div>
        </div>
    </header>
   
</template>

<script>
   export default {
       methods: {
           show(){
               this.$emit("buttonCliked")
           }
       }
   }

</script>

<style scoped>

header 
{
    background: #464646
}
header button
{
    cursor: pointer;
}
header .nav-bar 
{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
}
   
</style>