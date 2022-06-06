<script>
    import { type, data } from '$lib/store.js';
    import Country from '$lib/component/quiz/Country.svelte';
    import Capital from '$lib/component/quiz/Capital.svelte';
    import Flag from '$lib/component/quiz/Flag.svelte';
</script>

<div class="quiz container py-5">
    <div class="row">
        <div class="offset-4 col-4">
            <div class="text-center">
                Q: {$type.question}<br>
                A: {$type.answer}
            </div>
        </div>
    </div>
</div>