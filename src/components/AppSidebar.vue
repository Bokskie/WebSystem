<template>
    <aside>
        <div class="sidebar">
            <h1>KAN<span>-ANAN</span></h1>
            <a href="">
                <span class="material-symbols-sharp">menu_book</span>
                <h3>Menu</h3>
            </a>

            <a href="">
                <span class="material-symbols-sharp">border_color</span>
                <h3>Order List</h3>
            </a>

            <a href="">
                <span class="material-symbols-sharp">assistant</span>
                <h3>About Us</h3>
            </a>

            <a href="">
                <span class="material-symbols-sharp">call</span>
                <h3>Contact</h3>
            </a>

    
            <a href="">
                <span class="material-symbols-sharp">logout</span>
                <h3>Log-Out</h3>
            </a>
        </div>
    </aside>
</template>

<style scoped>
*
{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    text-decoration: none;
    list-style: none;
}
aside
{
    background: #00aa6c;
    width: 250px;
    transition: all 0.5s ease;
}
aside .sidebar
{
    margin-top: 10px;
    display: flex;
    flex-direction: column;
}
aside .sidebar h1 
{
    text-align: center;
}
aside .sidebar span
{
    color: #ffffff;
}
aside .sidebar a 
{   
    display: flex;
    flex-direction: row;
    gap: 1rem;
    line-height: 6rem;
    padding-left: 4rem;
}
aside .sidebar a span
{
    color: #000;
    font-size: 30px;
    line-height: 6rem;
}
aside .sidebar a h3 
{
    font-size: 20px;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 200;
    color: #000;
}
aside .sidebar a:hover 
{
    background: #ffffff;
    border-top-left-radius: 2rem;
    border-bottom-left-radius: 2rem;
}
</style>
