<style>
    :root {
    --primary-color: rgb(162, 199, 224);
    --secodary-color: rgb(103, 170, 247);
}

* {
    box-sizing:  border-box;
}

main {
    display: flex;
    flex-wrap: wrap;
}

.movie {
    width: 300px;
    margin: 10px;
    background-color: var(--secodary-color);
    box-shadow: 0 4px 5px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
    border-radius: 3px;
}

.movie img{
    width: 100px;
}

.movie-info {
    color: black;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 15px 15px;
    letter-spacing: 0.5px;
}

.movie-info h3{
    margin-top: 0;
    margin-left: 10px;
    margin-right: 10px;
}

.movie-info span{
    background-color: var(--primary-color);
    padding: 25px 5px;
    border-radius: 3px;
    font-weight: bold;
}

.movie-info span.green{
    color: rgb(17, 131, 17);
}

.overview {
    background-color: white;
    padding: 20px;
    position: absolute;
    left: 0;
    bottom: 0;
    right: 0;
    max-width: 100%;
    transform: translateY(101%);
    transition: transform 0.3s ease-in;
}

.movie:hover .overview{
    transform: translateY(0)
}
</style>

<script>
	import Die_Hard from '$lib/images/Крепкий орешек.jpg';
    import Holop2 from '$lib/images/Холоп 2 (2023).webp';
    import TriBogatiry from '$lib/images/Три богатыря и Пуп Земли (2023).webp';
    import Cheburashka from '$lib/images/Чебурашка (2022).webp';
    import Challenge from '$lib/images/Вызов (2023).webp';
    import BigRace from '$lib/images/Большая гонка. Ауди против Лянчи (2024).webp';
</script>

<main id="main">
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src={Die_Hard} alt="Poster" />
            <h3 id="MovieTitle">Крепкий Орешек</h3>
            <span class="green">9.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">Описание фильма</h3>
            <a href="https://www.kinopoisk.ru/film/471/">Смотреть описание</a>
        </div>
    </div>

    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
			<img src={Holop2} alt="Poster" />
            <h3 id="MovieTitle">Холоп 2 (2023)</h3>
            <span class="green">7.2</span>
        </div>
        <div class="overview">
            <h3 id="Description">Описание фильма</h3>
            <a href="https://www.kinopoisk.ru/film/5047468/">Смотреть описание</a>
        </div>
    </div>
    
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
			<img src={TriBogatiry} alt="Poster" />
            <h3 id="MovieTitle">Три богатыря и Пуп Земли (2023)</h3>
            <span class="green">6.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">Описание фильма</h3>
            <a href="https://www.kinopoisk.ru/film/4489198/">Смотреть описание</a>
        </div>
    </div>

    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
			<img src={Cheburashka} alt="Poster" />
            <h3 id="MovieTitle">Чебурашка (2022)</h3>
            <span class="green">7.3</span>
        </div>
        <div class="overview">
            <h3 id="Description">Описание фильма</h3>
            <a href="https://www.kinopoisk.ru/film/4489198/">Смотреть описание</a>
        </div>
    </div>

    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
			<img src={Challenge} alt="Poster" />
            <h3 id="MovieTitle">Вызов (2023)</h3>
            <span class="green">7.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">Описание фильма</h3>
            <a href="https://www.kinopoisk.ru/film/4448519/">Смотреть описание</a>
        </div>
    </div>

    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
			<img src={BigRace} alt="Poster" />
            <h3 id="MovieTitle">Большая гонка. Ауди против Лянчи (2024)</h3>
            <span class="green">6.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">Описание фильма</h3>
            <a href="https://www.kinopoisk.ru/film/4965334/">Смотреть описание</a>
        </div>
    </div>
</main>