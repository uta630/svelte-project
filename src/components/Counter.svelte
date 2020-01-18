<script>
    export let count = 0, doubled, moreTimes;
    $: doubled = count * 2;
    $: moreTimes = doubled * 4;
    $: numbers = [count, doubled, moreTimes]
    $: sum = numbers.reduce((t, n) => t + n, 0);

    // $: console.log(`the count is ${count}`);
    // $: {
    //     console.log(`the count is ${doubled}`);
    //     console.log(`the count is ${moreTimes}`);
    // }
    $: if(count >= 100){
        console.log('over')
    } else {
        console.log(`the count is ${count}`);
    }

    function handleClick(){
        count += 1;
    }
</script>

<div class="c-btn" on:click={handleClick}>
    <p>counter : {count}</p>
    <p>doubled : {doubled}</p>
    <p>more times : {moreTimes}</p>
    <p>sum : {sum}</p>
</div>

<style lang="scss">
    .c-btn {
        display: inline-block;
        padding: 4px 6px;
        border: 1px solid #333;
        border-radius: 3px;
        cursor: pointer;
    }
</style>