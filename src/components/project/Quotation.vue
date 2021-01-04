<template>
    <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="panel panel-default">
                <div class="panel-default qupte">
                    <slot></slot>
                </div>
        </div>
    </div>
</template>

<style scoped>

/* .panel-body{
    font-family: Arial, Helvetica, sans-serif;
    font-size: 24px;
    color: #6e6e6e;
}

.quote{
    cursor: pointer;
}
quote:hover{
background-color: #ffe2e2;
} */

.quote{
    display: grid;
    grid-template-columns: repeat(3,1fr);
    grid-gap: 1rem;
}
.panel-body{
    border: 1px solid #ccc;
    background: #41b883;
    padding: 1rem;
    border-radius: 5px;
    text-align: center;
    position: relative;
    cursor: pointer;
}


</style>