<script>
    import { goto } from '$app/navigation';
    import { type } from '$lib/store.js';
    import Question from '$lib/component/index/Question.svelte';
    import Answer from '$lib/component/index/Answer.svelte';
</script>

<div class="index container py-5">
    <div class="row">
        <div class="offset-4 col-4">
            <div class="text-center">
                <h3>제시하기</h3>
                <Question bind:question="{$type.question}"/>
            </div>
            <div class="text-center mt-5">
                <h3>맞추기</h3>
                <Answer bind:question="{$type.question}" bind:answer="{$type.answer}"/>
            </div>
            <div class="text-center mt-5">
                <button type="button" class="btn btn-block btn-primary" on:click="{()=>goto('/quiz')}">
                    <i class="bi bi-play-fill"></i> 시작
                </button>
            </div>
        </div>
    </div>
</div>