<script lang="ts">

    import { page } from "$app/stores"

    type Language = "en" | "es" | "fr";

    const language = {
        en: {
            title: "What is your role?",
            description: "Select the role that best describes you."
        },
        es: {
            title: "¿Cuál es tu rol?",
            description: "Selecciona el rol que mejor te describe."
        },
        fr: {
            title: "Quel est votre rôle?",
            description: "Sélectionnez le rôle qui vous décrit le mieux."
        },
    }

    const {lang = "en"} = $page.params as {lang : Language};

    const greetings = language[lang as Language];
    
</script>

<h1>{greetings.title}</h1>
<p>{greetings.description}</p>