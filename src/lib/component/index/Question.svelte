<script>
	export let question = 'country';
</script>

<div class="btn-group">
	<input type="radio" class="btn-check" name="question" id="question-country" value="country" autocomplete="off" bind:group="{question}">
	<label class="btn btn-outline-primary" for="question-country"><i class="bi bi-globe"></i> 나라 이름</label>
	<input type="radio" class="btn-check" name="question" id="question-capital" value="capital" autocomplete="off" bind:group="{question}">
	<label class="btn btn-outline-primary" for="question-capital"><i class="bi bi-building"></i> 수도</label>
	<input type="radio" class="btn-check" name="question" id="question-flag" value="flag" autocomplete="off" bind:group="{question}">
	<label class="btn btn-outline-primary" for="question-flag"><i class="bi bi-flag"></i> 국기</label>
</div>