<script>
    import Question from '$lib/component/Question.svelte';
    import Answer from '$lib/component/Answer.svelte';
</script>

<div class="index container py-5">
    <div class="row">
        <div class="offset-4 col-4">
            <div class="text-center mt-5">
                <h2>제시하기</h2>
                <Question/>
            </div>
            <div class="text-center mt-5">
                <h2>맞추기</h2>
                <Answer/>
            </div>   
        </div>
    </div>
</div>