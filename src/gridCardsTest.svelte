<div class="gridContainer"> 
    <div class="gridItem">grid item 1</div>
    <div class="gridItem">grid item 2</div>
    <div class="gridItem">grid item 3</div>
    <div class="gridItem">grid item 1</div>
    <div class="gridItem">grid item 2</div>
    <div class="gridItem">grid item 3</div>
</div>



<style>
.gridContainer{
    display: grid;
    /* width: 20%; */
    grid-template-columns: auto auto auto;
    grid-template-rows: 150px 150px;

    background-color: bisque;
    grid-gap: 10px;
}
.gridItem{
    background-color: aquamarine;

}
</style>