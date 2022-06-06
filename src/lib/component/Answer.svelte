<style>
	i { display: block; font-size: 10rem; color: #fff; padding-bottom: 5rem; }
	.carousel-item { background-color: #123; }
</style>

<div id="answer-carousel" class="carousel slide">
	<div class="carousel-indicators">
		<button type="button" data-bs-target="#answer-carousel" data-bs-slide-to="0" class="active"/>
		<button type="button" data-bs-target="#answer-carousel" data-bs-slide-to="1"/>
		<button type="button" data-bs-target="#answer-carousel" data-bs-slide-to="2"/>
	</div>
	<div class="carousel-inner">
		<div class="carousel-item active">
			<i class="bi bi-globe"></i>
			<div class="carousel-caption d-none d-md-block">
				<h5>나라 이름</h5>
			</div>
		</div>
		<div class="carousel-item">
			<i class="bi bi-building"></i>
			<div class="carousel-caption d-none d-md-block">
				<h5>수도</h5>
			</div>
		</div>
		<div class="carousel-item">
			<i class="bi bi-flag"></i>
			<div class="carousel-caption d-none d-md-block">
				<h5>국기</h5>
			</div>
		</div>
	</div>
	<button type="button" class="carousel-control-prev" data-bs-target="#answer-carousel" data-bs-slide="prev">
		<span class="carousel-control-prev-icon"/>
		<span class="visually-hidden">Previous</span>
	</button>
	<button class="carousel-control-next" type="button" data-bs-target="#answer-carousel" data-bs-slide="next">
		<span class="carousel-control-next-icon"/>
		<span class="visually-hidden">Next</span>
	</button>
</div>