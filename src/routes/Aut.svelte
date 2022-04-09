<script>
    import Header from "../lib/Header.svelte";

    function autHandler() {
        
    }
</script>

<Header />

<form on:submit|preventDefault>
    <h3>ВХОД</h3>

    <div class="form-input">
        <label for="login">Логин</label>
        <input type="text" name="login" />
    </div>

    <div class="form-input">
        <label for="password">Пароль</label>
        <input type="password" name="password" />
    </div>

    <div class="buttons">
        <button on:click={autHandler}> Зарегистрироваться </button>
        <a href="/#/calc" class="enterb"> Войти </a>
    </div>
</form>

<style>
    :root {
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
            Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    }

    .form-input {
        display: grid;
        
        grid-template-columns: 1fr 3fr;
        align-items: center;
    }

    label {
        text-align: end;
        margin-right: 2rem;
        color: rgba(77,61,255,1);
        font-size: 16px;
        font-weight: 600;
    }

    form {
        display: grid;
        background-color: aliceblue;
        padding: 2rem 5rem;
        border-radius: 14px;
        gap: 2rem;
    }

    

    input,
    button, 
    a {
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: large;
        max-height: 3rem;
        border: 1px #252525 solid;
        padding: 0.5rem 1rem;
    }

    input {
        border-radius: 5px;
    }
    
    button,
    a {
        border-radius: 24px;
        width: 100%;
        border-radius: 54px;
    }

    button:hover {
    }

    .buttons{
        display: grid;
        grid-template-columns: 1.5fr 1fr;
        gap: 1rem;
    }
    .enterb{
        background-color: rgba(77,61,255,1);
        text-decoration: none;
       color: aliceblue;
    }
    h3 {
        text-align: center;
        color: rgba(77,61,255,1);
        font-size: 2rem;
        font-weight: 400;
        margin: 0rem;
    }
</style>
