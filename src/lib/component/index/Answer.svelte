<script>
	export let question = 'country';
	export let answer = 'capital';

	let disableCountry, disableCapital, disableFlag = question;

	$:disableCountry = question === 'country';
	$:disableCapital = question === 'capital';
	$:disableFlag = question === 'flag';

	$:if (question === answer) {
		answer = ['country', 'capital', 'flag'].filter(el => el !== question)[0];
	}
</script>

<div class="btn-group">
	<input type="radio" class="btn-check" name="answer" id="answer-country" value="country" autocomplete="off" bind:group="{answer}" disabled="{disableCountry}">
	<label class="btn btn-outline-success" for="answer-country"><i class="bi bi-globe"></i> 나라 이름</label>
	<input type="radio" class="btn-check" name="answer" id="answer-capital" value="capital" autocomplete="off" bind:group="{answer}" disabled="{disableCapital}">
	<label class="btn btn-outline-success" for="answer-capital"><i class="bi bi-building"></i> 수도</label>
	<input type="radio" class="btn-check" name="answer" id="answer-flag" value="flag" autocomplete="off" bind:group="{answer}" disabled="{disableFlag}">
	<label class="btn btn-outline-success" for="answer-flag"><i class="bi bi-flag"></i> 국기</label>
</div>