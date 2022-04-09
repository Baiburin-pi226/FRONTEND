<script>
    import Header from "../lib/Header.svelte";

    let sum = 0
</script>

<Header />

<main>
<h3>Введите данные для расчёта</h3>

<form>
    <div class="form-input">
        <label for="">Муницип. образование</label>
        <select>
            <option>г. Уфа 02</option>
            <option>г. Казань 16</option>
            <option>г. Москва 77</option>
            <option>г. Горно-Алтайск 04</option>
        </select>
    </div>

    <div class="form-input">
        <label for="">Тип недвижимости</label>
        <select>
            <option>Комната</option>
            <option>Квартира</option>
            <option>Жилой дом</option>
            <option>Машино-место</option>
            <option>Иное сдание / сооружение</option>
        </select>
    </div>

    <div class="form-input">
        <label for="">Кадровая стоимость объекта (₽)</label>
        <input type="number" />
    </div>

    <div class="form-input">
        <label for="">Налог на инвертариз. стоимости (₽)</label>
        <input type="number" />
    </div>

    <div class="form-input">
        <label for="">Площадь объекта (м²)</label>
        <input type="number" />
    </div>

    <div class="form-input">
        <label for="">Размер доли в проаве (1/* или 1)</label>
        <input type="text" />
    </div>
    
    <div class="form-input">
        <label for="">Переод владения (в мес. от 1 до 12)</label>
        <input type="number" min="1" max="12" />
    </div>

    <div class="form-input">
        <label for="">Число несовершеннолетних детей</label>
        <input type="number" />
    </div>

    <div class="form-input">
        <label for="">Имеются ли у вас льготы?</label>
        <div class="lgots">
            <div class="radio">
                <label for="">Да</label>
                <input type="radio" name="lgots" id="">
            </div>
            <div class="radio">
                <label for="">Нет</label>
                <input type="radio" name="lgots" id="">
            </div>
        </div>
    </div>

    <div class="form-input">
        <label for="">Введите размер льготы (%)</label>
        <input type="number" min="0" max="100" />
    </div>

   <div class="form-input">
        <label for="">Сумма к уплате:</label>
        <span>{sum} ₽</span>
    </div>


    <div class="buttons">
        <button> Сгенерировать PDF-файл </button>
        <button class="enterb" > Расчитать </button>
    </div>
</form>

</main>

<style>
    main {
        background: #fff;
        padding: 2rem;
        border-radius: 10px;
    }

    .radio {
        display: flex;
    }

    .lgots {
        display: flex;
        gap: 20px;
    }

    form {
        display: grid;
        gap: 10px;
    }

    input,
    select,
    button {
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: large;
        max-height: 3rem;
        border: 1px #252525 solid;
        padding: 0.5rem 1rem;
    }

    input,
    select {
        border-radius: 5px;
    }
    
    button {
        border-radius: 24px;
        width: 100%;
        border-radius: 54px;
    }

    .form-input {
        display: grid;
        
        grid-template-columns: 1fr 3fr;
        align-items: center;

        gap: 20px;
    }

    .buttons{
        display: grid;
        grid-template-columns: 1.5fr 1fr;
        gap: 1rem;
    }
</style>