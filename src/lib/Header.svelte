<script>
    import logo from "../assets/logo.png";
</script>

<header>
    <div class="title">
        <h1>Налоговый калькулятор</h1>
        <h2>Расчет налога на имущество физических лиц</h2>
    </div>
    <img src={logo} alt="Логотип УГАТУ" />
</header>

<style>
    header {
        display: flex;
        justify-content: flex-end;
        align-items: center;
        width: 100%;
    }
    .title {
        width: 100%;
        text-align: center;
        margin-left: 192px; 
        color: rgb(255, 255, 255);
    }
    h1 {
        font-size: 3.5rem;
        margin-bottom: 0.3em;
    }
    h2{
        font-size: 1.8rem;
        margin: 0;
    }
</style>
